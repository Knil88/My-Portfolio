<script>
export default{
    data() {
        return {
          //Array di oggetti con le competenze e descrizioni

            cards:[{

                'title':'HTML',

                'icon':'/html5.svg',

                'descripiton':'Ho seguito il corso di Full-Stack Web Development di Boolean, che comprende un modulo su HTML. Grazie al corso, ho acquisito le conoscenze fondamentali per creare pagine web utilizzando il linguaggio di markup. Il corso mi ha fornito esercizi pratici e progetti per consolidare le mie competenze e sviluppare la mia creatività. Nel complesso, il corso mi ha permesso di diventare un professionista del settore informatico e di acquisire le competenze necessarie per sviluppare applicazioni web complete.' },

                {

                'title':'Css',

                'icon':'/css3-alt.svg',

                'descripiton':"Il corso di Full-Stack Web Development di Boolean include un modulo dedicato all'apprendimento di CSS, che mi ha permesso di acquisire le conoscenze fondamentali per formattare e personalizzare l'aspetto visivo delle pagine web. Grazie alle lezioni video e agli esercizi pratici, ho imparato a utilizzare le proprietà di CSS per modificare lo stile delle pagine, come la scelta dei colori, il layout, la tipografia e l'animazione. Inoltre, il corso mi ha fornito un'ampia conoscenza degli strumenti di sviluppo web utilizzati per creare siti web professionali. " },

                {
                'title':'Bootstrap',

                'icon':'/bootstrap.svg',

                'descripiton':"Il corso mi ha fornito le conoscenze fondamentali per utilizzare Bootstrap, un framework di sviluppo front-end per creare pagine web responsive e ben progettate in modo efficiente. Grazie alle lezioni video e agli esercizi pratici, ho imparato a utilizzare i componenti di Bootstrap per creare layout flessibili, barre di navigazione, moduli, tabelle, pulsanti, icone e molto altro ancora. Il corso mi ha anche fornito una conoscenza approfondita delle best practice per il design web. Nel complesso, il corso di Full-Stack Web Development di Boolean mi ha permesso di acquisire le competenze necessarie per utilizzare Bootstrap in modo efficace e diventare un professionista del settore informatico." },

                {

                'title':'sass',

                'icon':'/sass.svg',

                'descripiton':"Il corso di Full-Stack Web Development di Boolean include un modulo sull'utilizzo di Sass, un preprocessore CSS che mi ha permesso di creare fogli di stile più efficienti e gestibili. Grazie alle lezioni video e agli esercizi pratici, ho imparato a utilizzare Sass per organizzare meglio il mio codice CSS, definire variabili, utilizzare mixin, creare funzioni, utilizzare i controlli di flusso e altro ancora. Inoltre, il corso mi ha fornito una conoscenza approfondita delle tecniche avanzate di CSS, consentendomi di creare fogli di stile personalizzati e di alta qualità. " },

                {

                'title':'Javascript',

                'icon':'/js.svg',

                'descripiton':"Il corso di Full-Stack Web Development di Boolean include un modulo sull'utilizzo di JavaScript, il linguaggio di scripting più comune utilizzato per aggiungere funzionalità interattive alle pagine web. Grazie alle lezioni video e agli esercizi pratici, ho imparato i fondamenti di JavaScript, come le variabili, le funzioni, i cicli e le istruzioni condizionali, e ho acquisito competenze avanzate come l'utilizzo di oggetti, metodi, callback, promesse e asincronia. Inoltre, il corso mi ha fornito una conoscenza approfondita dei framework JavaScript più popolari, come React e Node.js, consentendomi di creare applicazioni web avanzate e scalabili." },

                {

                'title':'Vue.js',

                'icon':'/vue.svg',

                'descripiton':"Il corso di Full-Stack Web Development di Boolean include un modulo sull'utilizzo di Vue.js, un framework JavaScript utilizzato per la creazione di interfacce utente avanzate. Grazie alle lezioni video e agli esercizi pratici, ho imparato a utilizzare i concetti fondamentali di Vue.js, come le direttive, le proprietà computate e i cicli di vita dei componenti. Inoltre, il corso mi ha fornito una conoscenza approfondita delle funzionalità avanzate di Vue.js, come la gestione degli eventi, l'uso di componenti dinamici, la comunicazione tra i componenti e la creazione di animazioni e transizioni." },

                {

                'title':'node',

                'icon':'/node.svg',

                'descripiton':"Il corso di Full-Stack Web Development di Boolean include un modulo sull'utilizzo di Node.js, un ambiente di runtime JavaScript utilizzato per la creazione di applicazioni web lato server. Grazie alle lezioni video e agli esercizi pratici, ho imparato a utilizzare i concetti fondamentali di Node.js, come il sistema di moduli, il file system e i processi, e ho acquisito competenze avanzate come l'utilizzo di Express, un framework per la creazione di applicazioni web in Node.js. Inoltre, il corso mi ha fornito una conoscenza approfondita dei concetti di sicurezza, autenticazione e autorizzazione nelle applicazioni web, nonché delle tecniche per il testing e il debug delle applicazioni Node.js." },

                {

                'title':'php',

                'icon':'/php.svg',

                'descripiton':"l corso di Full-Stack Web Development di Boolean include un modulo sull'utilizzo di PHP, un linguaggio di scripting ampiamente utilizzato per la creazione di applicazioni web lato server. Grazie alle lezioni video e agli esercizi pratici, ho imparato a utilizzare i concetti fondamentali di PHP, come le variabili, i cicli, le funzioni e le classi. Inoltre, il corso mi ha fornito una conoscenza approfondita delle funzionalità avanzate di PHP, come la gestione delle sessioni, la connessione ai database MySQL e l'utilizzo di framework per la creazione di applicazioni web moderne." },

                {

                'title':'laravel',

                'icon':'/laravel.svg',

                'descripiton':"Il corso di Full-Stack Web Development di Boolean include un modulo sull'utilizzo di Laravel, un framework PHP per la creazione di applicazioni web. Grazie alle lezioni video e agli esercizi pratici, ho imparato a utilizzare le funzionalità di base di Laravel, come l'architettura Model-View-Controller (MVC), le migrazioni del database e le relazioni tra i modelli. Inoltre, il corso mi ha fornito una conoscenza approfondita delle funzionalità avanzate di Laravel, come la gestione degli eventi, la creazione di API RESTful e l'implementazione di autenticazione e autorizzazione. Inoltre, il corso mi ha mostrato come integrare Laravel con altre tecnologie web come Vue.js e Bootstrap per creare applicazioni web moderne e performanti." },
            ]
        }
    },
}

</script>

<template>
  <!-- Sezione competenze -->

  <section id="Skills">

    <div class="container px-4 py-5 text-white" id="hanging-icons">

        <h2 class="pb-2 border-bottom">my skills</h2>

        <div class="row g-4 py-5 row-cols-1 row-cols-lg-3" >

          <div class="col d-flex align-items-start" v-for="card in cards">

            <div class="icon-square bg-transparent  flex-shrink-0 me-3 ">

              <div class="container_ico" >

                <img :src="card.icon" alt="">

              </div>

            </div>

            <div>

              <h2>{{card.title}}</h2>

              <p class="paragrap_h">{{ card.descripiton }}</p>

            </div>

          </div>
       
        </div>

      </div>  
      
  </section>
    
</template>

<style lang="scss">
.container_ico img {

    
    min-height: 41px;
    filter: invert(80%) ;
   
}
.paragrap_h{
  color: #09d99a;
  border: 10px solid whitesmoke;
  background-color: black;
  font-family: 'Anonymous Pro', monospace;
  padding: 15px;
  font-size: 14px;
  max-height: 250px;
  overflow-y: scroll;
}
</style>
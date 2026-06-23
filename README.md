
<!DOCTYPE>
<html>
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width,inital-scale=1.0">
    
    <title> Vue Example</title>
    
    <script src="https://unpkg.com/vue@3"></script> <!--CDN-->
    
    <body>
      <div id="app">
        
        <p><input type="text" v-model="message"></p>
        <p>{{message}} 
            ({{message.length}}) </p>

  
      </div>   
      <script>
      Vue.createApp({
        data() {
          return{
            message: 'Nagkaon kana lab?'
          }
        },
        mounted (){
          setTimeout(() => {
            this.message = 'sorry gid ba, banha gid ni sila';
          },3000);
        }
        
      }).mount('#app');
      
      </script>
      
    </body>
  
    
  </head> 
</html>

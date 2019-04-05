# Peter-Mary
<html lang="en">
  <head> 56
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />

    <title>Mini App</title>

    <style>
      
      body {
        background: lavender;
      }
      
      div.user-photo {
        width: 150px;
        height: 150px;
        margin: 1em auto;
        background: #fff;
      }
      
      div.details {
        font-size: 2.3em;
        margin: 2.5em 0.2em 0.2em 0.2em;
        color: #fff;
        padding: 1.1em;
      }
      
      footer {
        width: calc(100% - 2em);
        z-index: 500;
        position: absolute;
        bottom: 0;
        overflow: hidden;
        display: flex;
        justify-content: space-between;
        margin: 0 1em;
      }
      
      footer button.mdc-icon-button {
        margin: 0.5em;
      }
      
    </style>
  </head>
  <body>
    
    <script>
      
      const notify = (msg) => {
        const toastr = document.querySelector('.messages');
        if(!toastr) return;
        
        toastr.textContent = msg;
        if(!toastr.classList.contains('on')) {
          toastr.classList.add('on');
        }
      };
      
      const clearNotice = () => {
        const toastr = document.querySelector('.messages');
        if(!toastr) return;
        
        toastr.textContent = '';
        toastr.classList.remove('on');
      };
      
      const displayUserPhotoAndName = (data) => {
        if(!data) return;
        
        // add your code here

        clearNotice();
      };
            
      const getAUserProfile = () => {
        const api = 'https://randomuser.me/api/';
        
        // make API call here
        
        notify(`requesting profile data ...`);
      };
      
      const startApp = () => {
        // invoke the getAUserProfile here
      };

      startApp();
    </script>
  </body>
</html>

<template>
    <v-container id="contactForm">
      
        <v-subheader class="text-center justify-center py-6">
            <h3 class="font-weight-bold text-h3 font_color">
                Contact
            </h3>
        </v-subheader>
        <v-container id="form">
            <h3>Let's Collaborate</h3>
            <p>Please use the form below to contact me for my resume, 
              job opportunities, or to discuss and collaborate! Feel free to email me as well @ 
              <a href="mailto:eric.stretton@gmail.com">eric.stretton@gmail.com</a>
            </p>

            <form id="action" action="https://formsubmit.co/eric.stretton@gmail.com" method="POST"></form>
              <input class="inputColor" type="text" name="name" placeholder="Name" required>
              <input class="inputColor" type="email" name="email" placeholder="Email" required>
              <input class="inputColor" type="text" name="company" placeholder="Company (Optional)" >
              <textarea class="inputColor" name="content" placeholder="A brief message here..." required></textarea>
              <v-btn
              id="submit"
              type="submit"
              >Send</v-btn>
        </v-container>
      
    </v-container>
</template>

<script>
 

  
  export default {
    name: "ContactMe",
    data() {
      return {
        name: '',
        email: '',
        company: '',
        content: ''
      }
    }
    
  }
</script>

<style lang="scss" scoped>

#contactForm{
  display: grid;
  justify-items: center;
  height: fit-content;
  width: 100vw;

  #form{
    widows: 100%;
    height: fit-content;
    margin: 3vh;
    padding: 15px;
    background-color: #343030;
    border: 2px solid whitesmoke;
    border-radius: 5px;
    .inputColor{
      color: whitesmoke;
      opacity: 0.75;
    }
    p, h3{
      opacity: 0.75;
      color: whitesmoke;
      a{
        color: whitesmoke;
      }
    }
    #action{
      margin: 5%;
      display: grid;
      justify-items: center;

      input, textarea{
        margin: 2%;
        width: 100%;
        padding: 5px;
        border-radius: 5px;
        
      }
      textarea{
        height: 125px;
      }
    }
    #submit{
      background-color: #488fef;
      color: whitesmoke;
      display: block;
      width: 8vw;
      justify-self: end;
    }
  }
  .font_color{
      color: #6aaaff;
  }
}



    @media screen and (min-width: 700px) {
            #contactForm {
                #form {
                    width: 625px;
                    h3 {
                        margin-bottom: 2vh;
                    }
                    #action {
                        margin-top: 3vh;
                    }
                }
            }
        }
    @media screen and (min-width: 1100px) {
        #contactForm {
            #form {
                width: 80%;
                display: grid;
                p {
                    width: 75%;
                    justify-self: center;
                }
            }
        }
    }
</style>
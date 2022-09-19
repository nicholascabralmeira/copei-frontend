<template>

  <div>

    <!-- carousel com imagens -->

    <section>
      <b-carousel>
        <b-carousel-item>
          <b-image class="image" src="https://picsum.photos/id/431/1230/300"></b-image>
        </b-carousel-item>
        <b-carousel-item>
          <b-image class="image" src="https://picsum.photos/id/432/1230/300"></b-image>
        </b-carousel-item>
        <b-carousel-item>
          <b-image class="image" src="https://picsum.photos/id/433/1230/300"></b-image>
        </b-carousel-item>
      </b-carousel>
    </section>
    <section class="section mt-4">

      <div class="columns is-multiline">
        <div v-for ="grupo in grupos" :key="grupo.nome"   class="column is-3">
          <div>
              <h2 class="title is-2 has-text-centered">{{grupo.nome}}</h2>


              <div v-for="selecao in grupo.selecoes" :key="selecao.nome" class="buttons">
                <b-button type="is-primary" expanded>
                  <img style="height: 30px;"
                    :src="selecao.bandeira"
                    alt="">
                  {{selecao.nome}}
                </b-button>
              </div>
            </div>
        </div>
      </div>     
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      grupos: [
        {
          nome: "Grupo A",
          selecoes: [
            {
              nome: "Qatar",
              bandeira: "https://cdn.iconscout.com/icon/free/png-256/qatar-flag-country-nation-union-empire-33060.png"
            },
            {
              nome: "Equador",
              bandeira: "https://cdn.iconscout.com/icon/free/png-256/qatar-flag-country-nation-union-empire-33060.png"
            },

            {
              nome: "Senegal",
              bandeira: "https://cdn.iconscout.com/icon/free/png-256/qatar-flag-country-nation-union-empire-33060.png"
            },

            {
              nome: "Holanda",
              bandeira: "https://cdn.iconscout.com/icon/free/png-256/qatar-flag-country-nation-union-empire-33060.png"
            }
          ]
        },

        {
          nome: "Grupo B",
          selecoes: [
            {
              nome: "Inglaterra",
              bandeira: "https://cdn.iconscout.com/icon/free/png-256/qatar-flag-country-nation-union-empire-33060.png"
            },

            {
              nome: "Iran",
              bandeira: "https://cdn.iconscout.com/icon/free/png-256/qatar-flag-country-nation-union-empire-33060.png"
            },

            {
              nome: "Estados Unidos",
              bandeira: "https://cdn.iconscout.com/icon/free/png-256/qatar-flag-country-nation-union-empire-33060.png"
            },

            {
              nome: "Pais de Gales",
              bandeira: "https://cdn.iconscout.com/icon/free/png-256/qatar-flag-country-nation-union-empire-33060.png"
            }

          ]
        },

        {
          nome: "Grupo C",
          selecoes: [
            {
              nome: "Argentina",
              bandeira: "https://cdn.iconscout.com/icon/free/png-256/qatar-flag-country-nation-union-empire-33060.png"
            },

            {
              nome: "Arabia Saudita",
              bandeira: "https://cdn.iconscout.com/icon/free/png-256/qatar-flag-country-nation-union-empire-33060.png"
            },

            {
              nome: "Mexico",
              bandeira: "https://cdn.iconscout.com/icon/free/png-256/qatar-flag-country-nation-union-empire-33060.png"
            },

            {
              nome: "Polonia",
              bandeira: "https://cdn.iconscout.com/icon/free/png-256/qatar-flag-country-nation-union-empire-33060.png"
            }

          ]
        },

        {
          nome: "Grupo D",
          selecoes: [
            {
              nome: "Franca",
              bandeira: "https://cdn.iconscout.com/icon/free/png-256/qatar-flag-country-nation-union-empire-33060.png"
            },

            {
              nome: "Australia",
              bandeira: "https://cdn.iconscout.com/icon/free/png-256/qatar-flag-country-nation-union-empire-33060.png"
            },

            {
              nome: "Dinamarca",
              bandeira: "https://cdn.iconscout.com/icon/free/png-256/qatar-flag-country-nation-union-empire-33060.png"
            },

            {
              nome: "Tunisia",
              bandeira: "https://cdn.iconscout.com/icon/free/png-256/qatar-flag-country-nation-union-empire-33060.png"
            }

          ]
        },

        {
          nome: "Grupo D",
          selecoes: [
            {
              nome: "Franca",
              bandeira: "https://cdn.iconscout.com/icon/free/png-256/qatar-flag-country-nation-union-empire-33060.png"
            },

            {
              nome: "Australia",
              bandeira: "https://cdn.iconscout.com/icon/free/png-256/qatar-flag-country-nation-union-empire-33060.png"
            },

            {
              nome: "Dinamarca",
              bandeira: "https://cdn.iconscout.com/icon/free/png-256/qatar-flag-country-nation-union-empire-33060.png"
            },

            {
              nome: "Tunisia",
              bandeira: "https://cdn.iconscout.com/icon/free/png-256/qatar-flag-country-nation-union-empire-33060.png"
            }

          ]
        },

        {
          nome: "Grupo D",
          selecoes: [
            {
              nome: "Franca",
              bandeira: "https://cdn.iconscout.com/icon/free/png-256/qatar-flag-country-nation-union-empire-33060.png"
            },

            {
              nome: "Australia",
              bandeira: "https://cdn.iconscout.com/icon/free/png-256/qatar-flag-country-nation-union-empire-33060.png"
            },

            {
              nome: "Dinamarca",
              bandeira: "https://cdn.iconscout.com/icon/free/png-256/qatar-flag-country-nation-union-empire-33060.png"
            },

            {
              nome: "Tunisia",
              bandeira: "https://cdn.iconscout.com/icon/free/png-256/qatar-flag-country-nation-union-empire-33060.png"
            }

          ]
        },

        {
          nome: "Grupo D",
          selecoes: [
            {
              nome: "Franca",
              bandeira: "https://cdn.iconscout.com/icon/free/png-256/qatar-flag-country-nation-union-empire-33060.png"
            },

            {
              nome: "Australia",
              bandeira: "https://cdn.iconscout.com/icon/free/png-256/qatar-flag-country-nation-union-empire-33060.png"
            },

            {
              nome: "Dinamarca",
              bandeira: "https://cdn.iconscout.com/icon/free/png-256/qatar-flag-country-nation-union-empire-33060.png"
            },

            {
              nome: "Tunisia",
              bandeira: "https://cdn.iconscout.com/icon/free/png-256/qatar-flag-country-nation-union-empire-33060.png"
            }

          ]
        },

        {
          nome: "Grupo D",
          selecoes: [
            {
              nome: "Franca",
              bandeira: "https://cdn.iconscout.com/icon/free/png-256/qatar-flag-country-nation-union-empire-33060.png"
            },

            {
              nome: "Australia",
              bandeira: "https://cdn.iconscout.com/icon/free/png-256/qatar-flag-country-nation-union-empire-33060.png"
            },

            {
              nome: "Dinamarca",
              bandeira: "https://cdn.iconscout.com/icon/free/png-256/qatar-flag-country-nation-union-empire-33060.png"
            },

            {
              nome: "Tunisia",
              bandeira: "https://cdn.iconscout.com/icon/free/png-256/qatar-flag-country-nation-union-empire-33060.png"
            }

          ]
        }

      ]
    }
  },
  methods: {
  }
}
</script>


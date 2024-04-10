<template>
<div id="footmind">
    <div class="container d-flex ">
        <div id="list">
            <ul class="list-unstyled mx-2 " v-for="(item, index) in menufooter" :key="index">
                <li>
                    <h3 class="text-white">{{ item.title }}</h3>
                </li>
                <li v-for="(item, index) in item.links" :key="index">{{ item.text }}</li>
            </ul>
        </div>
        <div id="dc-comics"></div>
    </div>
</div>
</template>


<script>
export default {
  name: 'FooterMid',
  data() {
    return {
      menufooter: [
        {
          title: 'DC Comics', // Capitalized 'Comics' for consistency
          links: [
            {
              text: 'Characters' // Replaced 'dc' with 'text' for clarity
            },
            {
              text: 'Comics'
            },
            {
              text: 'Movies'
            },
            {
              text: 'TV'
            },
            {
              text: 'Games' // Added missing links
            },
            {
              text: 'Videos'
            },
            {
              text: 'News'
            },
          ],
        },
        {
          title: 'Shop',
          links: [
            {
              text: 'Shop DC'
            },
            {
              text: 'Shop DC Collectibles'
            }
          ]
        },
        {
          title: 'DC',
          links: [
            {
              text: 'Terms of Use' // Capitalized for clarity
            },
            {
              text: 'Privacy Policy (New)' // Added parenthesis
            },
            {
              text: 'Ad Choices'
            },
            {
              text: 'Advertising'
            },
            {
              text: 'Jobs'
            },
            {
              text: 'Subscriptions'
            },
            {
              text: 'Talent Workshops'
            },
            {
              text: 'CPSC Certificates'
            },
            {
              text: 'Ratings'
            },
            {
              text: 'Shop Help'
            },
            {
              text: 'Contact Us' // Capitalized for clarity
            },
          ]
        },
        {
          title: 'Sites',
          links: [
            {
              text: 'DC'
            },
            {
              text: 'MAD Magazine'
            },
            {
              text: 'DC Kids'
            },
            {
              text: 'DC Universe'
            },
            {
              text: 'DC Power Visa'
            },
          ]
        },
      ]
    };
  }
};
</script>

<style lang="scss" scoped>

    #footmind {
        
        background-image: url('/img/footer-bg.jpg');
   

        #list {
            width: 50%;
            display: flex;

            li {
                color: grey
            }
        }

        #dc-comics {
            width: 50%;
            background-image: url('/img/dc-logo-bg.png');
            background-position: center;
            background-repeat: no-repeat;
            background-size: 70%;

        }
    }

</style>
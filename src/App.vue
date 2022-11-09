<script setup>
import HelloWorld from './components/HelloWorld.vue'


import BarTest  from './components/bars/TestBar.vue'
import IconTest from './components/icons/TestIcon.vue'
import ButtonTest from './components/buttons/TestButton.vue'


function log(msg) {  
    alert(msg)
}
</script>

<template>
    <header>
        <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />

        <div class="wrapper">
            <HelloWorld msg="You did it!" />
        </div>
    </header>

    <main>
        <BarTest>
            <template #icon>
                <IconTest icon="profile-icon.svg"></IconTest>
            </template>
            
            Title Big mob
              
            <template #button>
                <ButtonTest :class="btn" @click="log('Button works!')">Label Mob</ButtonTest> 
            </template>
        </BarTest>
    </main>
</template>



<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}
main{
    justify-content: center;
    align-items: center;
    display: flex;
    padding: 20px 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
 
}
</style>

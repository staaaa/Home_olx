<template>
    <div class="wrapper">
        <h2>WITAMY W AUCTION STORE</h2>
        <p>Zarejestruj konto, aby korzystać z serwisu.</p>
        <div class="form-wrapper">
            <form action="" @submit.prevent="">
                <VInput class="input" type="text" placeholder="PODAJ EMAIL" href="../../static/assets/icons/at-solid.svg"/>
                <VInput class="input" type="text" placeholder="PODAJ NAZWE UŻYTKOWNIKA" href="../../static/assets/icons/user-solid.svg"/>
                <VInput class="input" type="password" placeholder="PODAJ HASŁO" href="../../static/assets/icons/lock-solid.svg"/>
                <VInput class="input" type="password" placeholder="POTWIERDŹ HASŁO" href="../../static/assets/icons/lock-solid.svg"/>
                <VButton class="input submit" value="ZAREJESTRUJ KONTO"/>
            </form>
            <VLine class="input line"/>
            <router-link to="/login">
                <p class="subtext">MASZ JUŻ KONTO? ZALOGUJ SIĘ TUTAJ</p>
            </router-link>
            <router-link to="/">
                <p class="subtext second">POWRÓT NA STRONĘ GŁÓWNĄ</p>
            </router-link>
        </div>
    </div>
</template>
<script>
import VInput from '../components/Input.vue'
import VButton from '../components/Button.vue'
import VLine from '../components/Line.vue'

export default {
    components:{
        VInput,
        VButton,
        VLine,
    }
}
</script>
<style scoped>
@media screen and (min-width: 600px){
.form-wrapper{
    width:600px;
    margin:auto;
}
}
h2{
    margin-top:20px;
}
h2, p{
    text-align:center;
    font-family:'Red Hat Display';
    font-weight: 700;
    padding:10px 0;
}
.subtext{
    margin-top:5px;
    font-size:0.75rem;
}
.input{
    margin-top:20px;
    margin-left:auto;
    margin-right:auto;
}
.submit, .line{
    margin-top:60px;
}
.line{
    margin-bottom:25px;
}
.second{
    text-decoration:underline;
}
</style>
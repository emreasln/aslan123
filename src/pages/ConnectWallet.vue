<template>
    <div class="home-blog backgroup-body button-top-style-">
        <Header />
        <ConnectWallet />
        <Footer />

    </div>
</template>

<script>
import Header from '../components/Header/Header'
import ConnectWallet from '../components/ConnectWallet/ConnectWallet'
import Footer from '../components/Footer/Footer'


export default {
    name: 'Home01',
    components: {
        Header,
        ConnectWallet,
        Footer,
    }
}
</script>
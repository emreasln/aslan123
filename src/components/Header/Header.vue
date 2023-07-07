<template>

        <header :class="['header', { 'is-fixed': isSticky }]" id="header_main">
     
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <div class="header__body">
                        <div class="header__logo">
                            <a href="/">
                                <img id="site-logo" src="../../assets/images/logo/logo-main.png" alt="SatStarter" width="165" height="40" data-retina="assets/images/logo/logo-main@x2.png" data-width="165" data-height="40">
                            </a>
                        </div>
                        <div class="header__right">
                            <nav id="main-nav" class="main-nav" v-bind:class="{active: isActive}">
                                <ul id="menu-primary-menu" class="menu">
                                    <li class="menu-item" @click="toggleActiveMobile()" v-bind:class="{active: inActiveMobile}">
                                        <a href="#">Home</a>       
                                    </li>
                                    <li class="menu-item" @click="toggleActiveMobile1()" v-bind:class="{active: isActiveMobile1}">
                                        <router-link to="connect-wallet">IDO</router-link>
                                        <ul class="sub-menu" >
                                        </ul>
                                    </li>
                                    <li class="menu-item">
                                        <router-link to="https://satstarter.gitbook.io/doc/">Whitepaper</router-link>
                                    </li>
                                
                                      
                                    <li class="menu-item " @click="toggleActiveMobile4()" v-bind:class="{active: isActiveMobile4}">
                                        <router-link to="#">Apply</router-link>
                                
                                
                                    </li>
                                </ul>
                            </nav>
                            <div class="group-button">
                                <router-link class="btn-action" to="/connect-wallet">
                                    <span>CONNECT WALLET</span>
                                </router-link>
                            </div>
                             <div class="mobile-button" @click="toggleActive()" v-bind:class="{active: isActive}" ><span></span></div>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        </header>  

</template>

<script>

import "./styles.scss";

export default {
    name: "Header",
    data() {
        return {
            isSticky: false,
            isActive: false,
            isActiveMobile:false,
            isActiveMobile1:false,
            isActiveMobile2:false,
            isActiveMobile3:false,
            isActiveMobile4:false,
            isActiveMobile5:false,
            search: false,
            Header: null,
            HeaderImg: null,
        };
    },
    mounted() {
        const that = this;
        window.addEventListener("scroll", () => {
            let scrollPos = window.scrollY;
            if (scrollPos >= 100) {
                that.isSticky = true;
            } else {
                that.isSticky = false;
            }
        });
    },
    methods: {
        isSideMenuMethod(isSideMenu){
            return this.isSideMenu = !isSideMenu
        },
        toggleActive(){
            this.isActive = !this.isActive;
        },
        toggleActiveMobile(){
            this.isActiveMobile = !this.isActiveMobile;
        },
        toggleActiveMobile1(){
            this.isActiveMobile1 = !this.isActiveMobile1;
        },
        toggleActiveMobile2(){
            this.isActiveMobile2 = !this.isActiveMobile2;
        },
        toggleActiveMobile3(){
            this.isActiveMobile3 = !this.isActiveMobile3;
        },
        toggleActiveMobile4(){
            this.isActiveMobile4 = !this.isActiveMobile4;
        },
        toggleActiveMobile5(){
            this.isActiveMobile5 = !this.isActiveMobile5;
        },
         toggleActiveSearch(){
            this.search = !this.search;
        },
    },
};
</script>

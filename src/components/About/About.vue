
<template>
    <section class="about style-1 mobie-pb0">
        <div class="container">
            <div class="row">
                <div class="col-xl-7 col-md-12">
                    <div class="about__image">
                    <img src='../../assets/images/layout/Graphic.png' alt="Image" />
                    </div>
                </div>
                <div class="col-xl-5 col-md-12">
                    <div class="about__content">
                        <div class="block-text">
                            <h3 class="title">What is SatStarter?</h3>
                            <p>SatStarter, the premier launchpad and incubator for the thriving Bitcoin Ordinals and BRC-20 ecosystem,
                                 offers an all-in-one platform for innovative projects in the BTC ecosystem. By introducing DeFi elements like DEX, lending and farming, we empower the Bitcoin community and foster growth.</p>
                        </div>

                        <div class="list-icon-box" data-aos="fade-up" data-aos-duration="800" >
                            <div class="icon-box" v-for="item in dataAbout.slice(0,3)" :key="item.id">
                                <div class="icon"><span :class="item.classAction" ></span></div>
                                <div class="content">
                                    <h5>{{item.title}}</h5>
                                    <p class="fs-14">{{item.content}}</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>

import "./styles.scss";

import { dataAbout } from '../../fake-data/data-about';

export default {
    name: "About",
     data (){
        return {
            dataAbout,
        }    
    },
};
</script>
            
            
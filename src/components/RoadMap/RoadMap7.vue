
<template>
    <section class="road-map style-7 mobie-pb0" id="roadmap">
        <div class="container">
            <div class="row">
                <div class="col-md-12">
                    <div class="block-text center">
                        <h2 class="heading">{{title}}</h2>
                        <p class="fs-20">{{desc}}</p>
                    </div>
                </div>
            </div>
        </div>
        <div class="container-fluid">
            <div class="row">
                <div class="col-md-12">
                    <div class="road-map__main" data-aos="fade-up" data-aos-duration="1000">
                    <carousel class="swiper-roadmap-7"
                            :settings='settings' 
                            :breakpoints='breakpoints'
                        >
                            <Slide v-for="slide in dataRoadMap.slice(36,45)" :key="slide.id">
                                <div class="box-roadmap" :class="slide.classAction">
                                    <p class="time">{{slide.title}}</p>
                                    <h5 class="title-box">{{slide.title2}}</h5>
                                    <div class="icon"></div>
                                    <svg width="18" height="211" viewBox="0 0 18 211" fill="none" xmlns="http://www.w3.org/2000/svg">
                                        <path fillRule="evenodd" clipRule="evenodd" d="M0 0V0.995283L1 0.995283V0H0ZM0 2.98585V4.97641H1L1 2.98585H0ZM0 6.96698V8.95755H1V6.96698H0ZM0 10.9481V12.9387H1L1 10.9481H0ZM0 14.9292V16.9198H1L1 14.9292H0ZM0 18.9104V20.9009H1L1 18.9104H0ZM0 22.8915V24.8821H1L1 22.8915H0ZM0 26.8726V28.8632H1L1 26.8726H0ZM0 30.8538V32.8443H1L1 30.8538H0ZM0 34.8349V36.8255H1L1 34.8349H0ZM0 38.816V40.8066H1L1 38.816H0ZM0 42.7972L1.95773e-06 44.7877H1V42.7972H0ZM2.04474e-06 46.7783L2.13176e-06 48.7689H1L1 46.7783H2.04474e-06ZM2.21877e-06 50.7594L2.30578e-06 52.75H1V50.7594H2.21877e-06ZM2.39279e-06 54.7406L2.4798e-06 56.7311H1L1 54.7406H2.39279e-06ZM2.56681e-06 58.7217L2.65382e-06 60.7123H1V58.7217H2.56681e-06ZM2.74083e-06 62.7028L2.82784e-06 64.6934H1L1 62.7028H2.74083e-06ZM2.91485e-06 66.684L3.00186e-06 68.6745H1L1 66.684H2.91485e-06ZM3.08887e-06 70.6651L3.17588e-06 72.6556H1L1 70.6651H3.08887e-06ZM3.26289e-06 74.6462L3.3499e-06 76.6368H1L1 74.6462H3.26289e-06ZM3.43691e-06 78.6273L3.52392e-06 80.6179H1L1 78.6273H3.43691e-06ZM3.61093e-06 82.6085L3.69794e-06 84.599H1L1 82.6085H3.61093e-06ZM3.78495e-06 86.5896L3.87196e-06 88.5801H1V86.5896H3.78495e-06ZM3.95897e-06 90.5707L4.04598e-06 92.5613H1L1 90.5707H3.95897e-06ZM4.13299e-06 94.5518L4.22e-06 96.5424H1V94.5518H4.13299e-06ZM4.30701e-06 98.533L4.39402e-06 100.524H1L1 98.533H4.30701e-06ZM4.48103e-06 102.514L4.56804e-06 104.505H1V102.514H4.48103e-06ZM4.65505e-06 106.495L4.74206e-06 108.486H1L1 106.495H4.65505e-06ZM4.82907e-06 110.476L4.91608e-06 112.467H1V110.476H4.82907e-06ZM5.00309e-06 114.457L5.09011e-06 116.448H1.00001L1.00001 114.457H5.00309e-06ZM5.17711e-06 118.439L5.26413e-06 120.429H1.00001L1.00001 118.439H5.17711e-06ZM5.35114e-06 122.42L5.43815e-06 124.41H1.00001L1.00001 122.42H5.35114e-06ZM5.52516e-06 126.401L5.61217e-06 128.391H1.00001L1.00001 126.401H5.52516e-06ZM5.69918e-06 130.382L5.78619e-06 132.373H1.00001L1.00001 130.382H5.69918e-06ZM5.8732e-06 134.363L5.96021e-06 136.354H1.00001L1.00001 134.363H5.8732e-06ZM6.04722e-06 138.344L6.13423e-06 140.335H1.00001V138.344H6.04722e-06ZM6.22124e-06 142.325L6.30825e-06 144.316H1.00001L1.00001 142.325H6.22124e-06ZM6.39526e-06 146.307L6.48227e-06 148.297H1.00001V146.307H6.39526e-06ZM6.56928e-06 150.288L6.65629e-06 152.278H1.00001L1.00001 150.288H6.56928e-06ZM6.7433e-06 154.269L6.83032e-06 156.259H1.00001V154.269H6.7433e-06ZM6.91733e-06 158.25L7.00434e-06 160.241H1.00001L1.00001 158.25H6.91733e-06ZM7.09135e-06 162.231L7.17836e-06 164.222H1.00001L1.00001 162.231H7.09135e-06ZM7.26537e-06 166.212L7.35238e-06 168.203H1.00001L1.00001 166.212H7.26537e-06ZM7.43939e-06 170.193L7.5264e-06 172.184H1.00001L1.00001 170.193H7.43939e-06ZM7.61341e-06 174.175L7.70042e-06 176.165H1.00001L1.00001 174.175H7.61341e-06ZM7.78743e-06 178.156L7.87444e-06 180.146H1.00001L1.00001 178.156H7.78743e-06ZM7.96145e-06 182.137L8.04846e-06 184.127H1.00001L1.00001 182.137H7.96145e-06ZM8.13547e-06 186.118L8.22248e-06 188.109H1.00001L1.00001 186.118H8.13547e-06ZM8.3095e-06 190.099L8.39651e-06 192.09H1.00001V190.099H8.3095e-06ZM8.48352e-06 194.08L8.57053e-06 196.071H1.00001L1.00001 194.08H8.48352e-06ZM8.65754e-06 198.061L8.74455e-06 200.052H1.00001V198.061H8.65754e-06ZM8.83156e-06 202.042L8.91857e-06 204.033H1.00001L1.00001 202.042H8.83156e-06ZM9.00558e-06 206.024L9.09259e-06 208.014H1.00001V206.024H9.00558e-06ZM1.00001 210.005H0.9V210H0V211H0.9H1.00001V210.005ZM2.7 211H4.5V210H2.7V211ZM6.3 211H8.1V210H6.3V211ZM9.9 211H11.7V210H9.9V211ZM13.5 211H15.3V210H13.5V211ZM17.1 211H18V210H17.1V211Z" fill="white"/>
                                    </svg>
                                    <ul class="list">
                                        <li v-for="text in slide.list" :key="text.id">
                                            <div class="dot"></div><p class="fs-17">{{text.text}}</p>
                                        </li>
                                    </ul>                           
                                </div>
                                
                            </Slide>
                            <template #addons>
                                <pagination />
                            </template>
                        </carousel>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import "./styles.scss";

import { defineComponent } from 'vue';
import { Carousel, Slide, Pagination,  } from 'vue3-carousel';

import 'vue3-carousel/dist/carousel.css';
import { dataRoadMap } from '../../fake-data/data-roadmap';


export default defineComponent ({
   name: "About3",
    components: {
        Carousel,
        Slide,
        Pagination,
    },
    data: () => ({
        dataRoadMap,
        desc: 'We’re slowly transforming the website into the best place for beginners to learn about cryptocurrencies.',
        title: 'ROADMAP',
        settings: {
            itemsToShow: 1,
            snapAlign: 'center',
        },
        breakpoints: {
            0: {
                itemsToShow: 1,
                snapAlign: 'center',
			},
            768: {
                itemsToShow: 2,
                snapAlign: 'center',
            },
            1024: {
                itemsToShow: 7,
                snapAlign: 'center',
            },
            1200: {
                itemsToShow: 7,
                snapAlign: 'center',
            },
        },
    }),
})

</script>
<template>
    <section class="section-faq style-1" id="faq">
        <div class="container">
            <div class="row">
                <div class="col-md-12">
                    <div class="block-text center">
                        <h3>{{title}}</h3>
                        <p class="mt-12">
                        {{subtitle}}
                        </p>
                    </div>

                    <div class="section-faq__main" data-aos="fade-up" data-aos-duration="800">
                        <div class="flat-tabs">
                            <Tab />
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

</template>

<script>

import Tab from "../Tab/Tab";
import "./styles.scss";


export default {
    name: 'Faq',
    data (){
        return {
            title: 'Have any Question? ',
            subtitle : 'Join the industry leaders to discuss where the markets are heading. We accept token payments',
        }    
    },
    components: {
        Tab,
    }
}
</script>
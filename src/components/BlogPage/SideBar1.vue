
<template>
    <div class="sidebar">
        <div class="widget widget-search">
            <form action="#">
                <input type="text" placeholder="Search Keyword" required="" />
                <button><svg width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M18.0885 16.9109L14.306 13.1283C15.2585 11.9217 15.8327 10.4026 15.8327 8.75008C15.8327 4.84425 12.6552 1.66675 8.74935 1.66675C4.84352 1.66675 1.66602 4.84425 1.66602 8.75008C1.66602 12.6559 4.84352 15.8334 8.74935 15.8334C10.4027 15.8334 11.921 15.2601 13.1277 14.3067L16.9102 18.0893C17.0727 18.2518 17.286 18.3334 17.4993 18.3334C17.7127 18.3334 17.926 18.2518 18.0885 18.0893C18.4144 17.7634 18.4144 17.2367 18.0885 16.9109ZM3.33268 8.75008C3.33268 5.76342 5.76268 3.33342 8.74935 3.33342C11.736 3.33342 14.166 5.76342 14.166 8.75008C14.166 11.7367 11.736 14.1667 8.74935 14.1667C5.76268 14.1667 3.33268 11.7367 3.33268 8.75008Z" fill="white"/>
                    </svg>
                    </button>
            </form>
        </div>
        <div class="widget widget-category">
            <h5 class="widget-title">
                Category
            </h5>
            <div class="content-widget">
                <ul class="form-check">
                    <li><input type="checkbox" class="form-check-input" id="exampleCheck1" />Blockchain</li>
                    <li><input class="form-check-input" type="checkbox" id="defaultCheck2" />Crypto</li>
                    <li><input class="form-check-input" type="checkbox" id="defaultCheck3" />Technology</li>
                    <li><input class="form-check-input" type="checkbox" id="defaultCheck4" />Random</li>
                </ul>
            </div>
        </div>
        <div class="widget widget-tags">
            <h5 class="widget-title">
                tags
            </h5>
            <div class="content-widget">
                <li v-for="item in dataSideBar" :key="item.id"><router-link :to="item.link">{{item.name}}</router-link></li>
            </div>
        </div>
    </div>
</template>

<script>

export default {
    name: "Feature",
     data (){
        return {
            dataSideBar: [
        {
            id: 1,
            name: 'Bitcoin',
            link: '#'
        },
        {
            id: 2,
            name: 'Ethereum',
            link: '#'
        },
        {
            id: 3,
            name: 'Released',
            link: '#'
        },
        {
            id: 4,
            name: 'Released',
            link: '#'
        },
        {
            id: 5,
            name: 'Coin',
            link: '#'
        },
        {
            id: 6,
            name: 'ICO',
            link: '#'
        },
        {
            id: 7,
            name: 'Tokens',
            link: '#'
        },
    ]
            }    
        }
    };
</script>
            
            
<template>
    <aside>
        <ul>
            <li>Promoções</li>
            <li>Brincos</li>
            <li>Colares</li>
            <li>Pulseiras</li>
        </ul>
    </aside>

    <div id="prodList">
        <div id="prod" v-for="(product, index) in products" :key="index">
            <img :src=product.url :alt=product.name>
            <p>{{product.name}}</p>
            <p>{{product.value}}</p>
        </div>
    </div>
    
</template>

<script>
export default {
    name: 'Products',
    data() {
        return {
            products: [
                {name:'anel1', value: 'R$45.00', url: require('@/assets/images/anel1.jpg')},
                {name:'anel2', value: 'R$65.00', url: require('@/assets/images/anel2.jpg')},
                {name:'anel3', value: 'R$55.00', url: require('@/assets/images/anel3.jpg')},
                {name:'anel4', value: 'R$42.00', url: require('@/assets/images/anel4.jpg')},
                {name:'anel5', value: 'R$38.00', url: require('@/assets/images/anel5.jpg')},
                {name:'anel6', value: 'R$61.00', url: require('@/assets/images/anel6.jpg')},
                {name:'anel7', value: 'R$53.00', url: require('@/assets/images/anel7.jpg')},
                {name:'brinco1', value: 'R$18.00', url: require('@/assets/images/brinco1.jpg')},
                {name:'brinco2', value: 'R$15.50', url: require('@/assets/images/brinco2.jpg')},
                {name:'brinco3', value: 'R$13.80', url: require('@/assets/images/brinco3.jpg')},
                {name:'brinco4', value: 'R$14.20', url: require('@/assets/images/brinco4.jpg')},
                {name:'colar1', value: 'R$95.00', url: require('@/assets/images/colar1.jpg')},
                {name:'colar2', value: 'R$82.00', url: require('@/assets/images/colar2.jpg')},
                {name:'pulseira1', value: 'R$31.00', url: require('@/assets/images/pulseira1.jpg')},
                {name:'pulseira2', value: 'R$33.00', url: require('@/assets/images/pulseira2.jpg')},
                {name:'pulseira3', value: 'R$34.50', url: require('@/assets/images/pulseira3.jpg')},
                {name:'pulseira4', value: 'R$38.70', url: require('@/assets/images/pulseira4.jpg')},
                {name:'pulseira5', value: 'R$40.80', url: require('@/assets/images/pulseira5.jpg')},
                {name:'pulseira6', value: 'R$61.00', url: require('@/assets/images/pulseira6.jpg')},
                {name:'pulseira7', value: 'R$51.00', url: require('@/assets/images/pulseira7.jpg')}

            ]
        }
    }
}
</script>

<style scoped>
    aside {
        position: absolute;
        padding: 20px;
        margin-top: 50px
    }

    ul {
        border: solid 1px black;
        width: 200px;
        background: #ffeffd;
    }

    li {
        width: 100%;
        display: block;
        transition: ease 0.5s;
        padding: 5px 0 5px;
        text-align: center;
    }

    li:hover {
        background: black;
        color: #ffeffd;
        cursor: pointer;
    }

    #prodList {
        float: right;
        display: block;
        width: 80%;
        padding: 40px 0 40px;
    }

    #prod {
        width: 18%;
        margin: 10px 1%;
        display: inline-block;
        height: 250px;
        background: #ffeffd;
        border-radius: 10px;
        box-shadow: 1px 2px 3px;
        transition: ease 0.5s;
    }

    #prod:hover {
        transform: scale(1.1);
        cursor: pointer;
    }

    #prod img {
        border-radius: 10px;
        width: 100%;
        height: 180px;
        margin: auto;
    }

    #prod p {
        font-size: 20px;
        text-align: center;
    }


</style>
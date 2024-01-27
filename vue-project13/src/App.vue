<template>
  <User v-for="user in arr" :key="user.id" :user="user"></User>

</template>

<script>
import User from './components/User.vue'

export default {
  components: {
    User
  },
  data(){
    return{
      arr: [
        {id: 1, name:'14.1" Ноутбук DEXP Aquilon серый', description:"Full HD (1920x1080), IPS, Intel Celeron N4020C, ядра: 2 х 1.1 ГГц, RAM 8 ГБ, SSD 256 ГБ, Intel UHD Graphics 600 , Windows 11 Home", price: "17 999 ₽"},
        {id: 2, name:'ПК DEXP Atlas H341', description:"Intel Celeron N4020, 2 x 1.1 ГГц, 4 ГБ DDR4, SSD 128 ГБ, без ОС", price: '7 999 ₽'},
        {id: 3, name:'Клавиатура проводная DEXP K-507BU', description:"мембранная, клавиш - 104, USB, черная", price: '499 ₽'},
        {id: 4, name:'Мини ПК Rombica Horizon J4 GKJ442D [PCMI-0002]', description:"Intel Celeron J4125, 4 x 2 ГГц, 4 ГБ LPDDR4, SSD 256 ГБ, без ОС", price: '19 499 ₽'},
        {id: 5, name:'23.8" Моноблок Prime Box Spirit PBI240-15/7305 N5095', description:"Intel Celeron N5095, 4x2 ГГц, IPS, Full HD (1920x1080), 8 ГБ DDR4, SSD 256 ГБ, Windows 11 Pro", price: '35 999 ₽'},
        {id: 6, name:'23.8" Моноблок DEXP AIO-MC [24HP8WP027]', description:"Intel Pentium Gold 7400, 2x3.7 ГГц, IPS, Full HD (1920x1080), 8 ГБ DDR4, SSD 256 ГБ, Windows 11 Pro", price: '40 999 ₽'},
        {id: 7, name:'Подставка для ноутбука Aceline LT-06B черный', description:"алюминий, пластик ", price: '250 ₽'},
        {id: 8, name:'ПО Р7-Офис. Редакторы документов для дома', description:"русский, BOX (карта с кодом), срок действия лицензии: 12 мес", price: '3 499 ₽'},
        {id: 9, name:'ПО Polaris Office Personal', description:"русский, ESD (электронный ключ), срок действия лицензии: неограниченно", price: '3 999 ₽'},
        {id: 10, name:'Микрокомпьютер ROCK Pi Model A 4GB RK3399', description:"Rockchip RK3399, 6 x 1800 МГц, RAM: 4096 МБ, LAN 1 Гбит/с", price: '9 799 ₽'},
      ],
    }
  },
  methods:{

  }
}
</script>

<style>

</style>


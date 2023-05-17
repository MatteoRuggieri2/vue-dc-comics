<template>
    <div class="container">
        <div class="wrapper">
            <span class="main-title">CURRENT SERIES</span>
            <SingleSeries v-for="(series, index) in card" :key="index" :SeriesObject="series" />
        </div>
        <a class="btn-lg-blue-bckg" href="#">LOAD MORE</a>
    </div>
</template>

<script>
import SingleSeries from "./SingleSeries";
export default {
    name: "MainContent",
    components: {
        SingleSeries
    },
    data: function() {
        return {
            card: [
                {
                    // "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                    "thumb": "https://static.dc.com/dc/files/default_images/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?w=640",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    // "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                    "thumb": "https://static.dc.com/dc/files/default_images/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?w=640",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    // "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                    "thumb": "https://static.dc.com/dc/files/default_images/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?w=640",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    // "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                    "thumb": "https://static.dc.com/dc/files/default_images/batgirl_v5_1_5b23e1f1124941.50950783.jpg?w=640",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    // "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "thumb": "https://static.dc.com/dc/files/default_images/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?w=640",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    // "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "thumb": "https://static.dc.com/dc/files/default_images/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?w=640",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    // "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                    "thumb": "https://static.dc.com/dc/files/default_images/BMSM_5d4361b7116261.74371456.jpg?w=640",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    // "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                    "thumb": "https://static.dc.com/dc/files/default_images/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?w=640",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    // "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                    "thumb": "https://static.dc.com/dc/files/default_images/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?w=640",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    // "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                    "thumb": "https://static.dc.com/dc/files/default_images/cover-v2_5f40314645a734.37285065.png?w=640",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    // "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                    "thumb": "https://static.dc.com/dc/files/default_images/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?w=640",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    // "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                    "thumb": "https://static.dc.com/dc/files/default_images/CATW_01_300-001_HD_5b7f28f98425a9.00783133.jpg?w=640",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ]
        };
    }
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';

    .container {
        text-align: center;
        padding-bottom: 20px;

        .wrapper {
            width: 100%;
            padding: 50px 0 10px;
            position: relative;
            display: flex;
            flex-wrap: wrap;

            .main-title {
                padding: 8px 30px;
                font-size: 30px;
                color: $secondary_color;
                background-color: $primary_color;
                position: absolute;
                top: 0;
                left: 0;
                transform: translateY(-50%);
            }
        }
    }

</style>
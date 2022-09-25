<template>
    <footer class="fs-5 text-white">

        <!-- TopFooter Component Reference -->
        <TopFooterComponent />

        <!-- Main footer -->
        <div class="main-footer">
            <div class="container d-flex justify-content-between">

                <!-- Footer Links -->
                <div class="col-4 d-flex py-4">

                    <!-- First column: Site navigation & Shops Links -->
                    <div class="col-4">
                        <LinkListComponent :listArray="dcNavLinks" />
                        <LinkListComponent :listArray="dcShops" />
                    </div>

                    <!-- Second column: DC Legal Links -->
                    <div class="col-4">
                        <LinkListComponent :listArray="dcLegals" />
                    </div>

                    <!-- Third column: DC Sites Links -->
                    <div class="col-4">
                        <LinkListComponent :listArray="sitesList" />
                    </div>

                </div>

                <!-- Logo nel background -->
                <div class="dc-footer-mark col-6">
                </div>

            </div>
        </div>

        <!-- BottomFooter Component Reference -->
        <BottomFooterComponent />

    </footer>
</template>


<script>
import BottomFooterComponent from '@/components/FooterComponents/BottomFooterComponent.vue';
import TopFooterComponent from '@/components/FooterComponents/TopFooterComponent.vue';
import LinkListComponent from '@/components/ComponentsUtils/LinkListComponent.vue';
export default {
    name: "FooterComponent",
    components: {
        BottomFooterComponent,
        TopFooterComponent,
        LinkListComponent,
    },
    data() {
        return {
            dcNavLinks: {
                title: 'DC Comics',
                elements: ['Characters', 'Comics', 'Movies', 'TV', 'Games', 'Videos', 'News']
            },
            dcShops: {
                title: 'Shop',
                elements: ['Shop DC', 'Shop DC Collectibles']
            },
            dcLegals: {
                title: 'DC',
                elements: ['Terms of Use', 'Privacy policy (New)', 'Ad Choices', 'Advertising', 'Jobs', 'Subscriptions', 'Talent Workshop', 'CPSC Certificates', 'Ratings', 'Shop Heplp', 'Contact Us']
            },
            sitesList: {
                title: 'Sites',
                elements: ['DC', 'MAD Magazine', 'DC Kids', 'DC Universe', 'DC Power Visa']
            }
        }
    }
}
</script>


<style lang="scss">
@import '@/assets/style/variables.scss';

// Main footer
.main-footer {
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;

    // Lista link
    ul {
        list-style-type: none;

        // Titolo lista
        li:first-child {
            color: white;
            font-weight: 400;
            text-transform: uppercase;

            cursor: default;
        }

        // Elementi lista
        li a {
            text-decoration: none;
            color: #ffffff5f;
            font-weight: 300;

            transition: color $tr-hover-transition;


            &:hover {
                color: $tr-dc-blue;
            }

        }


    }

    // Logo DC in background
    .dc-footer-mark {
        background-image: url(../assets/img/dc-logo-bg.png);
        background-position: center;
        background-repeat: no-repeat;
        background-size: auto;
    }

}
</style>
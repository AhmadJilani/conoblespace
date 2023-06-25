<template>
    <header id="header" class="border-bottom-0 dark" data-sticky-shrink="false">
        <div id="header-wrap">
            <div class="container">
                <div class="header-row">
                    <!-- Logo
						============================================= -->
                    <div id="logo">
                        <NuxtLink to="/">
                            <img
                                class="logo-default"
                                src="@/assets/images/logo-dark.png"
                                alt="Noble CoSpace logo"
                            />
                            <img
                                class="logo-sticky"
                                src="@/assets/images/logo-dark.png"
                                alt="Noble CoSpace logo"
                            />
                        </NuxtLink>
                    </div>
                    <!-- #logo end -->

                    <div class="header-misc">
                        <a class="top-phone" href="tel:+923238878361"
                            ><i class="fa-solid fa-phone"></i>
                            <span class="d-none d-md-inline-block"
                                >0323 8878361</span
                            ></a
                        >
                    </div>

                    <div class="primary-menu-trigger">
                        <button
                            class="cnvs-hamburger"
                            type="button"
                            title="Open Mobile Menu"
                        >
                            <span class="cnvs-hamburger-box"
                                ><span class="cnvs-hamburger-inner"></span
                            ></span>
                        </button>
                    </div>

                    <!-- Primary Navigation
						============================================= -->
                    <nav class="primary-menu">
                        <ul class="menu-container">
                            <li
                                class="menu-item"
                                :class="{ current: activeRoute === '/' }"
                            >
                                <NuxtLink class="menu-link" to="/"
                                    ><div>Home</div></NuxtLink
                                >
                            </li>
                            <li
                                class="menu-item"
                                :class="{ current: activeRoute === '/rates' }"
                            >
                                <NuxtLink class="menu-link" to="/rates"
                                    ><div>Rates</div></NuxtLink
                                >
                            </li>
                            <li
                                class="menu-item"
                                :class="{
                                    current: activeRoute === '/location',
                                }"
                            >
                                <NuxtLink class="menu-link" to="/location"
                                    ><div>Location</div></NuxtLink
                                >
                            </li>
                            <li
                                class="menu-item"
                                :class="{ current: activeRoute === '/contact' }"
                            >
                                <NuxtLink class="menu-link" to="/contact"
                                    ><div>Contact</div></NuxtLink
                                >
                            </li>
                        </ul>
                    </nav>
                    <!-- #primary-menu end -->
                </div>
            </div>
        </div>
        <div class="header-wrap-clone"></div>
    </header>
</template>

<script>
export default {
    name: "Header",
    computed: {
        activeRoute() {
            return this.$route.path;
        },
    },
};
</script>
<style lang="scss">
#logo img {
    height: 80px !important;
}
</style>

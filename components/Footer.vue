<template>
    <!-- Footer
		============================================= -->
    <footer id="footer" class="border-0 dark">
        <div class="container">
            <!-- Footer Widgets
    ============================================= -->
            <div class="footer-widgets-wrap dark pb-5">
                <div class="row">
                    <div class="col-lg-4 col-md-4">
                        <div class="widget">
                            <h4
                                class="ls-0 mb-4 text-transform-none text-white"
                            ></h4>

                            <NuxtLink to="/"
                                ><img
                                    src="@/assets/images/logo-text-dark.png"
                                    alt="Logo Footer"
                                    class="mb-4"
                                    height="60"
                            /></NuxtLink>
                            <p class="text-white-50">
                                affordable luxury coworking space
                            </p>
                            <a href="#" class="social-icon h-bg-facebook">
                                <i class="fa-brands fa-facebook-f"></i>
                                <i class="fa-brands fa-facebook-f"></i>
                            </a>
                            <a href="#" class="social-icon h-bg-twitter">
                                <i class="fa-brands fa-twitter"></i>
                                <i class="fa-brands fa-twitter"></i>
                            </a>
                            <a href="#" class="social-icon h-bg-instagram">
                                <i class="fa-brands fa-instagram"></i>
                                <i class="fa-brands fa-instagram"></i>
                            </a>
                        </div>
                    </div>
                    <div class="col-lg-2 col-md-2 col-6">
                        <div class="widget">
                            <h4
                                class="ls-0 mb-4 text-transform-none text-white"
                            >
                                Menu
                            </h4>

                            <ul class="list-unstyled ms-0">
                                <li class="mb-2">
                                    <NuxtLink to="/">Home</NuxtLink>
                                </li>
                                <li class="mb-2">
                                    <NuxtLink to="/rates">Rates</NuxtLink>
                                </li>
                                <li class="mb-2">
                                    <NuxtLink to="/location">Location</NuxtLink>
                                </li>
                                <li class="mb-2">
                                    <NuxtLink to="/contact">Contact</NuxtLink>
                                </li>
                            </ul>
                        </div>
                    </div>
                    <div class="col-lg-2 col-md-2 col-6">
                        <div class="widget">
                            <h4
                                class="ls-0 mb-4 text-transform-none text-white"
                            >
                                Forms
                            </h4>

                            <ul class="list-unstyled ms-0">
                                <li class="mb-2">
                                    <NuxtLink to="/forms/membership"
                                        >Membership Inquiry</NuxtLink
                                    >
                                </li>
                            </ul>
                        </div>
                    </div>
                    <div
                        class="col-md-4 col-12 d-flex align-items-center justify-content-center"
                    >
                        <h2 class="display-4 fw-semibold ls--2 text-center">
                            better
                            <span
                                class="text-rotater"
                                data-separator="|"
                                data-rotate="flipInX"
                                data-speed="3000"
                            >
                                <span class="t-rotate"
                                    >environment|workspace|coworking|community</span
                                >
                            </span>
                        </h2>
                    </div>
                </div>
            </div>
        </div>
        <!-- <img
            src="@/assets/images/lahore-silhouette.png"
            alt="Footer Image"
            class="footer-img w-100"
        /> -->
    </footer>
</template>

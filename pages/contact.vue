
<template>
    <div>
        <div class="container my-6">
            <div class="row justify-content-center text-center">
                <div class="col-md-8">
                    <h1 class="display-4 text-dark fw-semibold ls--2">
                        Contact Us
                    </h1>
                    <p>Reach out to us and we'll respond as soon as we can.</p>
                </div>
            </div>
        </div>


        <section class="section mb-0">
            <div class="container">
                <div class="row align-items-stretch col-mb-50 mb-0">
                    <div class="col-lg-6">
                        <div class="fancy-title title-border">
                            <h3>Send us an Email</h3>
                        </div>
                        <div id="app" class="form-widget">
                            <div class="form-result"></div>

                            <form
                            ref="form"
                                class="mb-0"
                                id="template-contactform"
                                name="template-contactform"
                                method="post"
                                action="https://docs.google.com/forms/d/e/1FAIpQLSdT-ePb2uAR-SHcgasCxeFajsdiEUezyEoeLxWwmLw4CAQ1bQ/formResponse"
                                novalidate="novalidate"
                            >
                                <div class="form-process">
                                    <div class="css3-spinner">
                                        <div class="css3-spinner-scaler"></div>
                                    </div>
                                </div>
                                <div class="row">
                                    <div class="col-md-12 form-group">
                                        <label for="entry.351062116"
                                            >Name <small>*</small></label
                                        >
                                        <input
                                        v-model="name"
                                            type="text"
                                            id="template-contactform-name"
                                            name="entry.351062116"
                                            value=""
                                            class="form-control required"
                                        />
                                    </div>
                                    <div class="col-md-12 form-group">
                                        <label for="entry.1095802241"
                                            >Email <small>*</small></label
                                        >
                                        <input
                                        v-model="email"
                                            type="email"
                                            id="template-contactform-email"
                                            name="entry.1095802241"
                                            value=""
                                            class="required email form-control"
                                        />
                                    </div>
                                    <div class="col-md-12 form-group">
                                        <label for="entry.1740074577"
                                            >Phone</label
                                        >

                                        <input
                                        v-model="phone"
                                            type="text"
                                            id="template-contactform-phone"
                                            name="entry.1740074577"
                                            value=""
                                            class="form-control"
                                        />
                                    </div>
                                    <div class="w-100"></div>
                                    <div class="col-md-12 form-group">
                                        <label
                                            for="entry.979820084"
                                            >Subject <small>*</small></label
                                        >
                                        <input
                                        v-model="subject"
                                            type="text"
                                            id="template-contactform-subject"
                                            name="entry.979820084"
                                            value=""
                                            class="required form-control"
                                        />
                                    </div>
                                    <div class="w-100"></div>
                                    <div class="col-12 form-group">
                                        <label
                                            for="entry.375415038"
                                            >Message <small>*</small></label
                                        >
                                        <textarea
                                        v-model="message"
                                            class="required form-control"
                                            id="template-contactform-message"
                                            name="entry.375415038"
                                            rows="6"
                                            cols="30"
                                        ></textarea>
                                    </div>
                                    <div class="col-12 form-group d-none">
                                        <input
                                            type="text"
                                            id="template-contactform-botcheck"
                                            name="template-contactform-botcheck"
                                            value=""
                                            class="form-control"
                                        />
                                    </div>
                                    <div class="col-12 form-group">
                                        <button
                                        @click="submitPage()"
                                            name="submit"
                                            type="submit"
                                            id="submit-button"
                                            tabindex="5"
                                            value="Submit"
                                            class="button button-3d m-0"
                                        >
                                            Send
                                        </button>
                                    </div>
                                </div>
                                <input
                                    type="hidden"
                                    name="prefix"
                                    value="template-contactform-"
                                />
                            </form>
                        </div>
                    </div>

                    <div class="col-lg-6 min-vh-50">
                        <div class="position-relative map-container">
                            <iframe
                                src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d13604.137429122837!2d74.317006!3d31.5232163!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x391905d79978b6fd%3A0x67ff390983c234db!2snoble%20cospace!5e0!3m2!1sen!2s!4v1687718596380!5m2!1sen!2s"
                                allowfullscreen
                                style="border: 0"
                                class="w-100 h-100"
                            ></iframe>
                        </div>
                    </div>
                </div>

                <div class="row col-mb-50 mb-4">
                    <div class="col-sm-6 col-lg-6">
                        <div
                            class="feature-box fbox-center fbox-bg fbox-plain border-secondary"
                        >
                            <div class="fbox-icon bg-light">
                                <NuxtLink to="/location"
                                    ><i class="uil uil-map-marker"></i
                                ></NuxtLink>
                            </div>
                            <div class="fbox-content">
                                <h3>
                                    Visit Us<span class="subtitle"
                                        >337, Rehmanpura, Lahore</span
                                    >
                                </h3>
                            </div>
                        </div>
                    </div>
                    <div class="col-sm-6 col-lg-6">
                        <div
                            class="feature-box fbox-center fbox-bg fbox-plain border-secondary"
                        >
                            <div class="fbox-icon bg-light">
                                <a href="tel:+923238878361"
                                    ><i class="bi-telephone"></i
                                ></a>
                            </div>
                            <div class="fbox-content">
                                <h3>
                                    Speak to Us<span class="subtitle"
                                        >0323 8878361</span
                                    >
                                </h3>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </div>
</template>
<script>

export default{
    data() {
        return{
            email: '',
    name: '',
    phone: '',
    subject:'',
    message:'',
        }

  },
  methods: {
        // resetForm() {
        //   this.$refs.form.reset();
        // },
        submitPage(){
            setTimeout( () => this.$router.push({ path: '/submission'}), 5000);
            setTimeout( ()=> this.$refs.form.reset(), 6000);


        }
      }


}

</script>

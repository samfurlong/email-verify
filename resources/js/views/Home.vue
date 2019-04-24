<template>
    <section class="hero is-primary is-medium main-hero">
        <div class="hero-body">
            <div class="container">
                <h1 class="title">
                    Email Verify
                </h1>
                <h2 class="subtitle">
                    Verify the deliverability of any email address with the most
                    complete email checker.
                </h2>

                <EmailVerifyComponent></EmailVerifyComponent>


            </div>
        </div>
    </section>
</template>

<script>
import EmailVerifyComponent from "../components/EmailVerifyComponent";

export default {
    components: { EmailVerifyComponent }
};
</script>

<style lang="scss">
.main-hero {
    text-align: center;
}
</style>

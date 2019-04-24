<template>
    <div class="box email-verify-box">
        <form @submit.prevent="onSubmit($event)">
            <div class="field has-addons">
                <div class="control is-expanded has-icons-left">
                    <input
                        class="input is-large"
                        type="email"
                        placeholder="johndoe@company.com"
                    />
                    <span class="icon is-medium is-left">
                        <i class="fas fa-envelope"></i>
                    </span>
                </div>
                <div class="control">
                    <button
                        type="submit"
                        :class="{ 'is-loading': loaded }"
                        class="button is-info is-large"
                    >
                        Verify
                    </button>
                </div>
            </div>
        </form>
    </div>
</template>

<script>
export default {
    data() {
        return {
            loaded: false
        };
    },
    mounted() {},
    methods: {
        onSubmit(event) {
            this.loaded = true;
        }
    }
};
</script>

<template>
    <div class="form-content">
        <div class="form-heading">
            <h2 class="form-heading-h2">Ihre Anfrage</h2>
        </div>
        <form class="form" @submit.prevent="submitForm">
            <div class="form-item">
                <label for="firstname">Vorname</label>
                <input class="form-input" type="text" id="firstname" name="firstname" v-model.trim="firstname"/>
            </div>
            <div class="form-item">
                <label for="lastname">Nachname</label>
                <input class="form-input" type="text" id="lastname" name="lastname" v-model.trim="lastname"/>
            </div>
            <div class="form-item"> 
                <label for="email">E-Mail</label>
                <input class="form-input" type="email" id="email" name="email" v-model.trim="email"/>
            </div>
            <div class="form-item">
                <label for="number">Telefonnummer</label>
                <input class="form-input" type="text" id="number" name="number" v-model.number="number"/>
            </div>
            <div class="form-item">
                <label for="description">Beschreibung</label>
                <textarea class="form-input" type="text" id="description" name="description" v-model.trim="description"></textarea>
            </div>
            <div class="form-submit">
                <form-button class="button-shadow" label="Absenden"></form-button>
            </div>
        </form>
    </div>
</template>

<script>
import FormButton from './UI/Buttons/FormButton.vue'

export default {
    components: {
        FormButton,
    },
    data() {
        return {
            firstname: '',
            lastname: '',
            email: '',
            number: '',
            description: ''
        }
    },
    methods: {
        submitForm() {
            console.log('Firstname: ' + this.firstname);
            this.firstname = '';

            console.log('Lastname: ' + this.lastname);
            this.lastname = '';

            console.log('E-Mail: ' + this.email);
            this.email = '';

            console.log('Number: ' + this.number);
            this.number = '';

            console.log('Description: ' + this.description);
            this.description = '';
        }
    }

}
</script>

<style scoped>
#description {
    min-width: 99%;
    max-width: 99%;
}

.form-heading {
    margin-bottom: 2rem;
}

.form-heading-h2 {
    font-size: 2rem;
}

.form-input {
    background-color: #3f455a;
    color: white;
    border: none;
    border-bottom: .1rem solid #8c1aff;
    border-radius: .65rem;
    height: 2rem;
}

.form-content {
    padding: 3rem 0;

    margin-top: 2rem;
    margin-bottom: 1rem;

    width: 75vw;
    background-color: #15171e;
    border-radius: .65rem;
}

.form-item {
    display: flex;
    flex-direction: column;
    text-align: left;
    justify-content: center;
    
    margin: 1rem auto;
    width: 25%;
}

.form-submit {
    margin-top: 1.75rem;

    position: relative;
}

@media(max-width: 1200px) {
    #description {
        min-width: 91%;
        max-width: 91%;
    }

    .form-content {
        margin-top: 0;
        width: 90%;
    }

    .form-item {
        width: 65%;
    }
}
</style>
<template>
  <div class="container mt-2">
    <b-form>
      <b-form-group 
        label="Título"
        label-for="subject"
      >
        <b-form-input
          id="subject"
          v-model="form.subject"
          type="text"
          placeholder="Ex: Lavar carro"
          required
          autocomplete="off"
        >
        </b-form-input>
      </b-form-group>

      <b-form-group 
        label="Descrição"
        label-for="description"
      >
        <b-form-textarea
          id="description"
          v-model="form.description"
          type="text"
          placeholder="Ex: Preciso levar o carro pra lavar"
          required
          autocomplete="off"
        ></b-form-textarea>
      </b-form-group>
      <b-button type="submit" variant="outline-primary">
        Salvar
      </b-button>
    </b-form>

  </div>
</template>

<script>
export default {
  name: "Form",

  data() {
    return {
      form: {
        subject: "",
        description: "",
      }
    }
  }
}
</script>

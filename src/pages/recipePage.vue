<template>
  <div>
    <div class="w-100 rounded-[12px]">
      <img src="/image-omelette.jpeg" class="img-fluid" alt="Omelette" />
    </div>
    <!-- Image -->
    <div class="mx-auto recipe-card">
      <!-- Title -->
      <h1 class="mb-3">Simple Omelette Recipe</h1>

      <p class="">
        An easy and quick dish, perfect for any meal. This classic omelette combines beaten eggs cooked to perfection, optionally filled with your choice of cheese, vegetables, or meats.
      </p>

      <!-- Preparation box -->
      <div class="prep-box p-3 rounded mb-4">
        <h3 class="mb-2">Preparation time</h3>
        <ul class="mb-0">
          <li><strong>Total:</strong> Approximately 10 minutes</li>
          <li><strong>Preparation:</strong> 5 minutes</li>
          <li><strong>Cooking:</strong> 5 minutes</li>
        </ul>
      </div>

      <!-- Ingredients -->
      <h3 class="section-title">Ingredients</h3>
      <ul>
        <li>2–3 large eggs</li>
        <li>Salt</li>
        <li>Pepper</li>
        <li>1 tbsp butter or oil</li>
      </ul>

      <!-- Instructions -->
      <h3 class="section-title">Instructions</h3>
      <ol>
        <li>Beat the eggs</li>
        <li>Heat the pan</li>
        <li>Cook the omelette</li>
        <li>Add fillings</li>
        <li>Fold and serve</li>
      </ol>

      <!-- Nutrition -->
      <h3 class="section-title">Nutrition</h3>

      <div class="row border-top py-2">
        <div class="col">Calories</div>
        <div class="col text-end fw-bold">277kcal</div>
      </div>
      <div class="row border-top py-2">
        <div class="col">Protein</div>
        <div class="col text-end fw-bold">20g</div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.recipe-card {
  max-width: 700px;
  padding: 30px;

  h1 {
    font-size: 2.2rem;
    };

    p {
      font-size: 1.18rem;
      color: #5f574e;
      margin-bottom: 2rem
    }
}

.prep-box {
  background: #fff5fa;
  padding: 24px;
  border-radius: 16px;
  
  h3 {
    color: #7b284f;
    font-size: 1.17rem;
  }

}

.section-title {
  margin-top: 1.5rem;
  font-weight: 700;
}
</style>

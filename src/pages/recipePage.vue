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
      <div class="prep-box">
        <h3 class="mb-2">Preparation time</h3>
        <ul class="mb-0">
          <li><span><strong>Total:</strong> Approximately 10 minutes</span></li>
          <li><span><strong>Preparation:</strong> 5 minutes</span></li>
          <li><span><strong>Cooking:</strong> 5 minutes</span></li>
        </ul>
      </div>

      <!-- Ingredients -->
      <section class="ingregrients">
        <h2 class="section-title">Ingredients</h2>
        <ul class="ingredient-list">
         <li><span>2–3 large eggs</span></li>
        <li><span>Salt, to taste</span></li>
        <li><span>Pepper, to taste</span></li>
        <li><span>1 tablespoon of butter or oil</span></li>
        <li><span>Optional fillings: cheese, diced vegetables, cooked meats, herbs</span></li>
        </ul>
      </section>

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
  border-radius: 8px;
  margin-bottom: 2em;

  h3 {
    color: #7b284f;
    font-size: 1.17rem;
  }

}

.section-title {
  font-weight: 500;
  color: #854632;
  margin-bottom: 1rem;
}

.ingregrients {
  margin-bottom: 2rem;
}

.ingredient-list {
  list-style: none;
  padding-left: 0;

  li {
    position: relative;
    padding-left: 1.3em;
    margin-bottom: 0.5rem;
    color: #5f574e;

    span {
     display: block;
     margin-left: 20px;
     font-size: 1rem;
    }

    &::before {
      content: '';
      position: absolute;
      left: 0;
      top: 50%;
      transform: translateY(-50%);
      width: 4px;
      height: 4px;
      background-color: #854632;
      border-radius: 50%;
    }
  }
}
</style>

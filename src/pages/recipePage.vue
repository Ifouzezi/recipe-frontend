<template>
  <div class="page-wrapper">
  <div class="page-container">
    <div class="w-100 rounded-[12px] img-container">
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
      <div class="instructions">
        <h3 class="section-title">Instructions</h3>
         <ol>
          <li>
            <span>
              <strong>Beat the eggs:</strong> In a bowl, beat the eggs with a pinch of salt and pepper until they are well mixed. You can add a tablespoon of water or milk for a fluffier texture.
            </span>
          </li>
          <li>
            <span>
              <strong>Heat the pan:</strong> Place a non-stick frying pan over medium heat and add butter or oil.
            </span>
          </li>
          <li>
            <span>
              <strong>Cook the omelette:</strong> Once the butter is melted and bubbling, pour in the eggs. Tilt the pan to ensure the eggs evenly coat the surface.
            </span>
          </li>
          <li>
            <span>
              <strong>Add fillings (optional):</strong> When the eggs begin to set at the edges but are still slightly runny in the middle, sprinkle your chosen fillings over one half of the omelette.
            </span>
          </li>
          <li>
            <span>
              <strong>Fold and serve:</strong> As the omelette continues to cook, carefully lift one edge and fold it over the fillings. Let it cook for another minute, then slide it onto a plate.
            </span>
          </li>
          <li>
            <span>
              <strong>Enjoy:</strong> Serve hot, with additional salt and pepper if needed.
            </span>
          </li>
        </ol>
      </div>
      
      <!-- Nutrition -->
      <div class="nutrition">
        <h3 class="section-title">Nutrition</h3>
        <p class="text-muted">
          The table below shows nutritional values per serving without the additional fillings.
        </p>

        <div class="row py-2 p-nutrition">
          <div class="col">Calories</div>
          <div class="col text-start color-nutrition fw-bold">277kcal</div>
        </div>

        <div class="row border-top p-nutrition py-2">
          <div class="col">Carbs</div>
          <div class="col text-start color-nutrition fw-bold">0g</div>
        </div>

        <div class="row border-top p-nutrition py-2">
          <div class="col">Protein</div>
          <div class="col text-start color-nutrition fw-bold">20g</div>
        </div>

        <div class="row border-top p-nutrition py-2">
          <div class="col">Fat</div>
          <div class="col color-nutrition text-start fw-bold">22g</div>
        </div>
      </div>
    </div>
  </div>
  </div>
</template>

<style scoped>
@media (min-width: 1024px) {
  .page-wrapper {
    background: #f3e5d7;
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 60px 20px;
  }
}

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

  ul {
    padding-left: 12px;

    li {
      margin-bottom: 0.5rem;
      /* color: #7b284f; */
      font-size: 12px;

      span {
        display: block;
        /* margin-left: 20px; */
        font-size: 1rem;
      }

      strong {
        color: #854632;
        margin-left: 20px;
      }
    }
  }

}

.section-title {
  font-weight: 500;
  color: #854632;
  margin-bottom: 1rem;
}

.ingregrients {
  margin-bottom: 2rem;
  border-bottom: 1px solid #bcb8b8;
  padding-bottom: 12px;
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

.instructions {
  margin-bottom: 2rem;
  border-bottom: 1px solid #bcb8b8;
  padding-bottom: 12px;

  ol {
    padding-left: 20px;
   
    ::marker {
      color: #854632;
      font-weight: bold;
    }

    li {
      margin-bottom: 1rem;
      color: #5f574e;

      span {
        display: block;
        margin-left: 20px;
        font-size: 1rem;
      }

      strong {
        color: #5f574e;
        /* margin-left: 20px; */
      }
    }
  }
}

.nutrition {
  .p-nutrition {
    padding-left: 36px;
    padding-right: 112px;

    .color-nutrition {
      color: #854632;
    }
  }
}

/* Desktop styles */
@media (min-width: 1024px) {
  h2, h3 {
    font-size: 1.5rem;
  }

  .page-container {
   background-color: white;
   max-width: 700px;
   border-radius: 24px;
   box-shadow: 0 4px 12px rgba(200, 200, 200, 0.1);
  }

  .img-container {
    padding: 32px 32px 0 32px;
    border-radius: 12px;
  }

  .img-fluid {
    border-radius: 12px;
  }

  /* Card container */
  .recipe-card {
    padding: 32px;
    
    h1 {
      font-size: 2rem;
    }

    p {
      font-size: 1rem;
    }
  }

  /* Image wrapper */
  .w-100 {
    
  }

  img {
   
  }

  /* Typography scaling */
  .recipe-card h1 {
   
  }

  .recipe-card p {
    
  }

  /* Preparation box spacing */
  .prep-box {
    
  }

  /* Section spacing */
  .ingregrients,
  .instructions {
    
  }

  /* Nutrition alignment */
  .nutrition .p-nutrition {
   
  }
}
</style>

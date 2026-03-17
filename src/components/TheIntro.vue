<script>
</script>

<template>
	<div class="intro">
		<div class="intro__content layout">
			<h2>
				I am an <span class="intro__emphasis">experienced product engineer</span>.
				Able to design high-quality solutions for backend and frontend systems with a strong overlap across cloud, infrastructure and data pipelines. Comfortable with incorporating LLMs into production enterprise software systems and utilising AI during development. Can perform as an independent contributor, cross-functional expert or a team lead.
			</h2>
		</div>
		<div></div>
	</div>
</template>

<style scoped lang="scss">
.intro {

  &__content {
    padding: 160px 0 120px;
  }

  &__emphasis {
    background-color: rgb(35, 35, 35);
    color: white;
    padding: 5px 10px;
  }
}

h2 {
  width: 50%;

  font-size: 1.8rem;
  text-align: justify;

  @media (max-width: $breakpoint-sm-max) {
    width: auto;

    font-size: 1.4rem;
    line-height: 2.5rem;
	}
}
</style>

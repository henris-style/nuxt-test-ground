<template>
	<main class="page page--home">
		<section class="intro">
			<div class="content">
				<p>Table should be white with black borders</p>
			</div>
			<div class="content">
				<div class="row grid-test">
					<div class="column small-half medium-third background--yellow">
						<h3>First column</h3>
						<p>This is the first column, which is yellow</p>
						<hr  >
						<p>Can you read this below? If so, thats good.</p>
						<p style="color: yellow">
							I'm a test text and should be readable, as in.. not have the same color text as the background.
						</p>
					</div>
					<div class="column small-half medium-third background--red">
						<h3>Second block</h3>
						<p>I'm actually a red block, but I should be shown as purple.</p>
					</div>
					<div class="column small-half medium-third background--blue">
						<h3>Fourth block</h3>
					</div>
					<div class="column small-half medium-third background--green hide-for-medium-up">
						<h3>I'm only visible on mobile.</h3>
					</div>
				</div>
			</div>
		</section>
	</main>
</template>

<script>
export default {
	components: {}
};
</script>

<style lang="scss">
@import '~tools';

.content {
	padding: 2rem;
	padding: grid(1);
}
.grid-test {
	border: 2px solid red;
	border: 2px solid color(Black);
	color: red;
	border-radius: 4px;
	color: color(Black);
	.column {
		padding: 1rem;
		padding: grid(0.5);
		border-right: 1px solid red;
		border-right: 1px solid color(Black);
		&:last-child {
			border: none;
		}
	}
}
</style>

<script>
	export let segment;

	export const text = 'button';
</script>

<style global>
</style>


<div class="mdc-slider" tabindex="0" role="slider"
     aria-valuemin="0" aria-valuemax="100" aria-valuenow="0"
     aria-label="Select Value">
  <div class="mdc-slider__track-container">
    <div class="mdc-slider__track"></div>
  </div>
  <div class="mdc-slider__thumb-container">
    <svg class="mdc-slider__thumb" width="21" height="21">
      <circle cx="10.5" cy="10.5" r="7.875"></circle>
    </svg>
    <div class="mdc-slider__focus-ring"></div>
  </div>
</div>
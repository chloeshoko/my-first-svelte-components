<script>
  let {
    title,
    text,
    ctaText,
    ctaHref,
  } = $props();
</script>

<aside class="promotional-aside" aria-labelledby="promo-title">
  <h2 id="promo-title" class="promo-title">{title}</h2>
  <p class="promo-text">{text}</p>
  <a class="promo-button" href={ctaHref}>{ctaText}</a>
</aside>

<style lang="scss">
  .promotional-aside {
    margin: var(--spacing-lg) 0;
    padding: var(--spacing-md);
    border: var(--border-width-thin) solid var(--color-border);
    border-left: var(--border-width-accent) solid var(--color-accent);
    background-color: var(--color-white);
    background-image: radial-gradient(var(--color-border) 1px, transparent 1px);
    background-size: 12px 12px;
  }

  .promo-title {
    margin: 0 0 var(--spacing-xs);
    font-family: var(--font-serif);
    font-size: var(--font-size-xl);
    font-weight: 700;
    line-height: 1.3;
    color: var(--color-dark);
  }

  .promo-text {
    margin: 0 0 var(--spacing-sm);
    font-size: var(--font-size-base);
    line-height: 1.6;
    color: var(--color-text);
  }

  .promo-button {
    display: inline-block;
    padding: 0.65rem 1rem;
    border-radius: 999px;
    font-family: var(--font-sans);
    font-size: var(--font-size-sm);
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 0.03em;
    color: var(--color-dark);
    background-color: var(--color-cuny-blue-light);
    text-decoration: none;
    border: var(--border-width-thin) solid var(--color-cuny-blue-light);
  }
</style>
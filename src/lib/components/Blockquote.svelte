<script>
  let { quote, attribution } = $props();
</script>

<blockquote>
  <p>{quote}</p>
  <cite>— {attribution}</cite>
</blockquote>

<style>
  blockquote {
    margin: 4rem 0;
    padding: 1.25rem 1.5rem;
    border: 1px solid var(--color-medium-gray);
    border-left: 6px double var(--color-dark);
    background-color: color-mix(in srgb, var(--color-light-gray) 65%, var(--color-white));
    box-shadow: inset 0 0 0 1px var(--color-border);
  }

  p {
    font-size: 1.25rem;
    line-height: 1.55;
    font-style: normal;
    font-family: var(--font-serif);
    color: var(--color-dark);
    letter-spacing: 0.005em;
  }

  cite {
    margin: 0.75rem 0 0;
    display: block;
    text-align: right;
    font-size: 0.875rem;
    font-weight: 700;
    font-style: normal;
    font-family: var(--font-serif);
    color: var(--color-medium-gray);
    text-transform: uppercase;
    letter-spacing: 0.08em;
  }
</style>
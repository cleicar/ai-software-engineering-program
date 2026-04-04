# Gemini Nano: executando uma LLM no navegador

This is a hands-on experiment to test Gemini Nano, Google's AI modeling technology, specifically designed to run locally on the user's computer.

### Local Processing (On Device)
Unlike ChatGPT or Gemini, which we access through a browser, Gemini Nano uses the user's own computer processor to generate responses.

- Privacy: Data does not leave your computer.

- Offline: Works without internet (after downloading the approximately 1.5 GB model).

- Latency: There is no network latency, although speed depends on your hardware.

---

### Browser Integration (Chrome Built-in AI)
What we are testing is a Google initiative to transform AI into a native browser tool, just like fetch() or console.log().

The idea is that, in the future, any web developer can use AI without having to pay for expensive APIs (like OpenAI's) or configure complex servers.

The browser comes with the "engine" (Gemini Nano) already installed.

---

### Testing different configurations

By manipulating the temperature and topK parameters, it's possible to observe the difference in the AI's behavior:
- With a temperature close to 0, the answer tends to be more predictable.
- With higher values, the AI ​​tends to be more creative.
- The topK defines how many candidates for the next token are considered.

For example: if we ask "The sky is..."
- With temperature=0, the answer will almost always be "blue".
- With temperature=2 and topK=10, the answer can vary to "vast", "unlimited", "full of stars", etc.
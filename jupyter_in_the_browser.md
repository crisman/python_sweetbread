
## Bits to build up the environment

[Wasm/WebAssembly](
https://en.wikipedia.org/wiki/WebAssembly
) (see also
[webassembly.org/](
https://webassembly.org/
)) which allows for (among many other things) running compiled code inside
a sandbox inside web browsers.

[https://emscripten.org/](
https://emscripten.org/
) toolchain using LLVM to create Wasm complied binaries.

[pyodide](
https://pyodide.org/en/stable/
) which is a "port of CPython to WebAssembly/Emscripten" that
"makes it possible to install and run Python packages in the browser".
[Python REPL in your browser](
https://pyodide.org/en/stable/console.html
).

[JupyterLite](
https://jupyterlite.readthedocs.io/en/latest/
) "is a JupyterLab distribution that runs entirely in the browser" using
(by default) pyodide to run the python bits in your browser. Where JupyterLab
is the new UI from Jupyter (marketing is "JupyterLab offers a more advanced,
feature rich, customizable experience compared to Jupyter Notebook.").

## Demo loading from JupyterLite docs site

See this in action with pretty graphs:

[altair example](
https://jupyterlite.readthedocs.io/en/latest/_static/lab/?path=pyodide/altair.ipynb
) should load a notebook starting with "Altair in JupyterLite"

To view pretty graphs:

- Open a `top` in some terminal to see high CPU usage in a moment
- Inside browser window, in Jupyter's top menu bar:
  - Click `Run`
    - Click `Run All Cells`
- watch things:
  - terminal `top` output for high usage in browser
  - On bottom bar of Jupyter, see `Python (Pyodide) | Busy` then `... | Idle`

## Docs for setting up under a web server

[JupyterLite your web server](
https://jupyterlite.readthedocs.io/en/latest/quickstart/standalone.html
)

[Local content on web server install](
https://jupyterlite.readthedocs.io/en/latest/quickstart/configure.html
)


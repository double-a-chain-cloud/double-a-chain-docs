# Double-A Chain Docs

**View conceptual documentation for the double-a chain project at [docs.acuteangle.com](https://docs.acuteangle.com)**.

## Working on this platform

To spin up a local instance, see below:

1. Install the python3 dependencies:

   ```shell
   wget http://cdn.npm.taobao.org/dist/python/3.6.5/Python-3.6.5.tgz
   tar -zxvf Python-3.6.5.tgz
   cd Python-3.6.5
   ./configure
   make clean
   make all
   ln -s /usr/local/bin/python3 /usr/bin/python3
   python3 --version
   ```

2. Install the Sphinx dependencies:

   ```shell
   python3 -m venv v-env
   source v-env/bin/activate
   pip install sphinx sphinx-autobuild sphinx_rtd_theme  recommonmark
   pip install sphinx_book_theme
   ```
3. make the `Double-A Chain docs`

   ```shell
   git clone https://github.com/double-a-chain-cloud/double-a-chain-docs
   cd double-a-chain-docs
   python3 -m venv v-env
   source v-env/bin/activate
   make html
   ```

4. Open `build/html/index.html` in your browser.

## License

All software code is copyright (c) acuteangle cloud, Inc. under the **MIT license**. Other written documentation and content is copyright (c) acuteangle cloud, Inc.
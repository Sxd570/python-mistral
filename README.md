Commands:
Requirement: python3.10

1. INSTALL llama-cpp-python PACKAGE
   > pip install --upgrade --quiet  llama-cpp-python
   
2. Download llama-cpp-python repository
    > git clone --recursive -j8 https://github.com/abetlen/llama-cpp-python.git
                           or
    extract the zip file
   
3. set the environment variable
   >set FORCE_CMAKE=1
   >set CMAKE_ARGS=-DLLAMA_CUBLAS=OFF

4. Compiling and installing
    Now you can cd into the llama-cpp-python directory and install the package
    > python -m pip install -e . --force-reinstall --no-cache-dir

5. Install langchain module in pip
    pip install langchain

6. Download the suitable model from hugging face, {CONSIDER YOUR SYSTEM RAM WHILE DOWNLOADING THE MODEL}
    > https://huggingface.co/TheBloke/Mistral-7B-Instruct-v0.1-GGUF

7. Paste the model in mistral folder

8. Open terminal and run 
    > python mistral.py

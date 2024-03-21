# background removal app with streamlit

This repo contains a background removal app built with streamlit. it allows users to upload images, remove the background while retaining high-quality resolution, and download the processed images.

![Screenshot 2024-03-21 113930](https://github.com/PranavBawgikar/streamlit-bg-remover/assets/102728016/3e452f15-c3c1-458e-b722-a3e985e9445e)
<br /> <br />
## installation

### running locally with python installed

to install the required dependencies, open your command prompt or terminal, navigate to the project directory, and run:

```bash
pip install -r requirements.txt
```

to run the app in your browser, execute the following command:

```bash
streamlit run bg_remove.py
```

### running on jupyter notebook or google colab

if you're working with jupyter notebook or google colab, you can install the required packages using the following commands:

```bash
pip install rembg==2.0.50
pip install Pillow==9.3.0
pip install streamlit==1.21.0
pip install numba==0.57
pip install numpy==1.23.0
```

1. you need to create a file, `app.py` (name can be anything) where you will write the streamlit code to run it on the web.

```bash
%%writefile app.py
```

3. use the following command to obtain your IPv4 address, which will serve as the tunnel password:

```bash
!wget -q -O - ipv4.icanhazip.com
```

3. after obtaining the IPv4 address, run the following command to set up a tunnel and access the streamlit app on the web:

```bash
streamlit run app.py & npx localtunnel --port 8501
```

4. the command will provide a URL. open that URL in your web browser and enter the IPv4 address as the tunnel password to access the streamlit app on the web.

## contributing

contributions are welcome! if you encounter any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.

## license

this project is licensed under the MIT license 💞

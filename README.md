# Docker for API

You can build and run the docker using the following process:

Cloning
```console
git clone https://github.com/jqueguiner/face-blurring.git face-blurring
```

Building Docker
```console
cd programming-language-detection && docker build -t face-blurring -f Dockerfile .
```

Running Docker
```console
echo "http://$(curl ifconfig.io):5000" && docker run -p 5000:5000 -d face-blurring
```

Calling the API
```console
curl -X POST "http://MY_SUPER_API_IP:5000/process" -H "accept: application/json" -H "Content-Type: application/json" -d '{"url":"https://i.ibb.co/FqDSQF8/input.jpg"}'
```

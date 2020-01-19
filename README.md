# Intel Openvino IoT Docker Image 


Create docker image and run it

```bash
git clone https://github.com/magrathj/IoT-Edge-App.git
sudo apt-get update && sudo apt-get upgrade
sudo apt-get install docker.io
systemctl start docker
systemctl enable docker
cd IoT-Edge-App
docker build . -t openvino
sudo docker ps
docker run -it openvino 
```

Check that you can run openvino demos

```bash
cd /opt/intel/openvino/deployment_tools/demo
./demo_squeezenet_download_convert_run.sh
```

Run the app on the test_video

```bash
python app.py -i test_video.mp4
```

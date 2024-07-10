# Deploy-app-to-GoogleKubernetesEngine
## Step:
- Build container image.
- Publish container image.
- Deploy ke Google Kubernetes Engine.
- Uji coba aplikasi.

### Build and Push Container Image
1. open **Cloud Shell**
2. **Type** following command to clone github repository
-     git clone https://github.com/DandiLesmana25/Bookshelf-Rest-API.git
3. build the application into a **Docker image**
   -     cd Bookshelf-Rest-API
   -     docker build -t bookhelfapp:0.1 .
4. Run the command below to display the Docker image:
   -     docker images
5.  Let's run this container application by running the following command:
   -     docker run -p 4000:8000 --name my-app bookhelfapp:0.1

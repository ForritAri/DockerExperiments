docker build -t ng_av .
docker run --name ng_avddd -d -p 8080:80 ng_av

# Til að mappa drif
docker run -v D:\dev\Python\nginxTest1\static-html-directory:/usr/share/nginx/html --name ng_avddd -d -p 8080:80 ng_av

# Clean up
docker rm -f ng_avddd

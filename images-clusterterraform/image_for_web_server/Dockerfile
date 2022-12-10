# alpine latest veersion en küçük boyutta linux kullanıyoruz.
# requirements.txt yi bulunduğumuz klasöre al. 
# requirements da bulunan flask ve flask-mysql uygulamalarını install ediyourz. Bunlar developerlardan alınır.
#  Bu şekilde, app.py dosyasında docuker rundan sonra bir değişiklik olsa da sadece app.py yi değiştirecek önceki adımları koruyacak
# copy ile dockerfile ın içerisinde bulunduğu klasordeki bütün dosyaları  root dizinde app diye bir kalsor oluşturup içine atıyorum.
## sonra bu app folderı working directoru haline getiriyourz
## expose 80 bir bilgi notu olarak bulunuyor 
# CMD ile docker run dedikten sonra container içindeki uygulamayı çalıştır.
FROM python:alpine
COPY requirements.txt .
RUN pip install -r requirements.txt
COPY . /app 
WORKDIR /app 
EXPOSE 80 
CMD python ./app.py 
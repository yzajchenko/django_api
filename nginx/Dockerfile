FROM nginx
# Удаляем дефолтный файл конфигураций
RUN rm /etc/nginx/conf.d/default.conf
COPY ./nginx.conf /etc/nginx/conf.d/
# Создаём папки в которых будут храниться
# статические и медиа файлы
RUN mkdir /todo
RUN mkdir /todo/static
RUN mkdir /todo/media
# Use the official NGINX image as the base image
FROM nginx:alpine

# Replace the default index.html with our own version containing a joke
RUN rm /usr/share/nginx/html/index.html && \
    echo '<!DOCTYPE html>' > /usr/share/nginx/html/index.html && \
    echo '<html>' >> /usr/share/nginx/html/index.html && \
    echo '  <head>' >> /usr/share/nginx/html/index.html && \
    echo '    <title>Joke</title>' >> /usr/share/nginx/html/index.html && \
    echo '  </head>' >> /usr/share/nginx/html/index.html && \
    echo '  <body>' >> /usr/share/nginx/html/index.html && \
    echo '    <h1>Why do programmers prefer dark mode?</h1>' >> /usr/share/nginx/html/index.html && \
    echo '    <p>Because light attracts bugs!</p>' >> /usr/share/nginx/html/index.html && \
    echo '  </body>' >> /usr/share/nginx/html/index.html && \
    echo '</html>' >> /usr/share/nginx/html/index.html

# Expose port 80 to allow access to NGINX
EXPOSE 80


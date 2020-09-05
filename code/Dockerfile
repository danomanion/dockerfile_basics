from ubuntu:18.04

COPY app /app
# ARG food
# ENV FOOD $food
# ENV NAME ItguyMichal
# ENV SURNAME=ItguyMichal, CITY=NewYork
# ADD app /app

WORKDIR /app
EXPOSE 8888

RUN apt-get update && apt-get install -y \
    python3 \
    python3-pip

# RUN echo $NAME
# RUN echo $SURNAME
# RUN echo $CITY
RUN pip3 install -r requirements.txt

# CMD ["jupyter lab", "--ip='0.0.0.0'", "--port=8888", "--no-browser", "--allow-root"]
CMD ["/bin/bash", "-c", "jupyter lab --ip='0.0.0.0' --port=8888 --no-browser --allow-root"]
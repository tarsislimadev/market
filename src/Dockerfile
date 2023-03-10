FROM tmvdl/android:app

WORKDIR /app

RUN cordova create market com.brtmvdl.market market

WORKDIR /app/market

COPY www/html www

RUN cordova platform add android

RUN cordova build android

FROM tmvdl/android:ionic

WORKDIR /app

RUN cordova create market com.brtmvdl.market market

WORKDIR /app/market

COPY www/html www

COPY ./config.xml ./config.xml

RUN cordova platform add android

RUN cordova plugin add cordova-plugin-barcodescanner

RUN cordova build android

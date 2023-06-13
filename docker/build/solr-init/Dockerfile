# escape=`


ARG PARENT_IMAGE
ARG SXA_IMAGE

FROM ${SXA_IMAGE} as sxa_image
FROM ${PARENT_IMAGE}

COPY --from=sxa_image c:\module\solr\cores-sxa.json c:\data\cores-sxa.json
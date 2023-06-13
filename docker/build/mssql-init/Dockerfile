# escape=`

ARG PARENT_IMAGE
ARG SPE_RESOURCES_IMAGE
ARG HEADLESS_SERVICES_IMAGE

FROM ${HEADLESS_SERVICES_IMAGE} AS headless_services
FROM ${SPE_RESOURCES_IMAGE} AS spe_resources_image
FROM ${PARENT_IMAGE}

# Copy and init the JSS / Headless Services Module
COPY --from=headless_services C:\module\db C:\resources\jss
COPY --from=spe_resources_image C:\module\db C:\resources\spe
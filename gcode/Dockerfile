FROM keyglitch/prusaslicer:2.3.0

LABEL "name"="Prusa Slicer gcode Action"
LABEL "maintainer"="Tideline3D <support@tideline3d.com>"
LABEL "version"="1.0.0"

LABEL "com.github.actions.name"="Prusa Slicer Action"
LABEL "com.github.actions.description"="Calls Prusa Slicer to generate gcode from STLs"
LABEL "com.github.actions.icon"="package"
LABEL "com.github.actions.color"="blue"

COPY entrypoint.sh /entrypoint.sh
COPY LICENSE-slic3r /

USER root

RUN apt-get update && apt-get install -y jq curl

ENTRYPOINT ["/entrypoint.sh"]

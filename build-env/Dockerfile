# DocDoku, Professional Open Source
# Copyright 2006 - 2017 DocDoku SARL
#
# This file is part of DocDokuPLM.
#
# DocDokuPLM is free software: you can redistribute it and/or modify
# it under the terms of the GNU Affero General Public License as published by
# the Free Software Foundation, either version 3 of the License, or
# (at your option) any later version.
#
# DocDokuPLM is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU Affero General Public License for more details.
#
# You should have received a copy of the GNU Affero General Public License
# along with DocDokuPLM.  If not, see <http://www.gnu.org/licenses/>.
#
## DocDokuPLM build environment
#
# Needed components:
#
# Java jdk8
# Node >= 8.x
# Maven 3
# Linux toolchain

FROM openjdk:8-jdk

RUN \
    curl -sL https://deb.nodesource.com/setup_8.x | bash - && \
    apt-get update && \
    apt-get install -y maven nodejs gcc make build-essential

# Allow dependency cache control
VOLUME ["/src", "/root/.m2", "/root/.npm"]
FROM azul/zulu-openjdk-alpine:21.0.4-21.36-jre-headless-x86
ARG DEPENDENCY=dependency
COPY ${DEPENDENCY}/BOOT-INF/lib /app/lib
COPY ${DEPENDENCY}/META-INF /app/META-INF
COPY ${DEPENDENCY}/BOOT-INF/classes /app
ENTRYPOINT ["java", "--enable-preview", "-Djdk.tracePinnedThreads", "-cp", "/app:/app/lib/*", "build.bazel.dashboard.Application"]

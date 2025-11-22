# Pull Request Title
Fix HMCL publish failing: produce jar before publishing

# Description
Fixes :HMCL:publishMavenPublicationToMavenLocalRepository failure (CI job ref: 1e345f3f6f7319f091a4f946fae97c625ef8a20a). Added publishing configuration to HMCL/build.gradle to ensure the jar task is executed and publication uses the jar produced by the current build. Also added dependsOn assemble for PublishToMavenLocal tasks.
Please review and merge.
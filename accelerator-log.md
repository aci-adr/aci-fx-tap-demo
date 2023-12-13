# Accelerator Log

## Options
```json
{
  "bsGitBranch" : "main",
  "bsGitRepository" : "github.com?owner=aci-adr&repo=aci-fx-tap-demo",
  "consumerName" : "STREAM_FX_DEMO_CONSUMER",
  "dbName" : "fx_data",
  "listenSubject" : "FX.DEMO",
  "natsUri" : "nats://10.0.217.253:4222",
  "projectName" : "aci-fx-tap-demo",
  "publishSubject" : "FX.DEMO.END",
  "stageName" : "aci-fx-tap-demo",
  "streamName" : "STREAM_FX_DEMO"
}
```
## Log
```
┏ engine (Chain)
┃  Info Running Chain(GeneratorValidationTransform, UniquePath)
┃ ┏ ┏ engine.transformations[0].validated (Combo)
┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ engine.transformations[0].validated.delegate (Chain)
┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0] (Merge)
┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Include
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.transformations[0].sources[0].delegate (Include)
┃ ┃ ┃ ┃ ┃  Info Will include [**]
┃ ┃ ┃ ┃ ┃ Debug .DS_Store matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug .idea/.gitignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug .idea/aci-adr-go-base.iml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug .idea/modules.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug .idea/vcs.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug .vscode/settings.json matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug Tiltfile matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug go.mod matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug go.sum matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug main.go matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug model/common/message.go matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug model/common/processing_info.go matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug model/entity/forex_data.go matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug service/.DS_Store matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug service/bal/event_handler.go matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug service/common/logger.go matched [**] -> included
┃ ┃ ┃ ┃ ┃ Debug service/dal/database.go matched [**] -> included
┃ ┃ ┃ ┃ ┗ Debug service/dal/mongodb_service.go matched [**] -> included
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.transformations[0].sources[1].delegate (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[1].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**/workload.yaml]
┃ ┃ ┃ ┃ ┃ ┃ Debug .DS_Store didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug .idea/.gitignore didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug .idea/aci-adr-go-base.iml didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug .idea/modules.xml didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug .idea/vcs.xml didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug .vscode/settings.json didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug Tiltfile didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug config/workload.yaml matched [**/workload.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug go.mod didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug go.sum didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug main.go didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug model/common/message.go didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug model/common/processing_info.go didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug model/entity/forex_data.go didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug service/.DS_Store didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug service/bal/event_handler.go didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug service/common/logger.go didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug service/dal/database.go didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┗ Debug service/dal/mongodb_service.go didn't match [**/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[1].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┗ ┗ ┗  Info Will replace [{{STREAM}}->STREAM_FX_DEMO, {{PUBLISH_SUBJECT}}->FX.DEMO.END, {{DB_NAME}}->fx_data, {{STAGE_NAME}}->aci-fx-tap-demo, {{LISTEN_SUBJECT}}->FX.DEMO, {{NATS_URI}}->nats://10.0.217.253:...(truncated), {{CONSUMER}}->STREAM_FX_DEMO_CONSU...(truncated)]
┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[1] (UniquePath)
┃ ┗ ┗ ┗ Debug Multiple representations for path 'config/workload.yaml', will use the one appearing last 
┗ ╺ engine.transformations[1] (UniquePath)
```

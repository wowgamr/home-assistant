####Point cleaning

```yaml
service: xiaomi_miot.call_action
data:
  entity_id: vacuum.roidmi_v60_9cd4_robot_cleaner
  did: xxxxxxxxx
  siid: 14
  aiid: 1
  params:
    - 4
    - "{\"MapId\":xxxxxxxxxx,\"ExtraAreas\":{\"vertexs\":[[651,10773],[2251,10773],[2251,9173],[651,9173]],\"mode\":\"point\"}}"
  throw: true
```

####Custom zone cleaning

```yaml
service: xiaomi_miot.call_action
data:
  entity_id: vacuum.roidmi_v60_9cd4_robot_cleaner
  did: xxxxxxxxx
  siid: 14
  aiid: 1
  params:
    - 2
    - "{\"MapId\":1652179690,\"ExtraAreas\":[{\"vertexs\":[[-664,12066],[641,12066],[641,13262],[-664,13262]],\"mode\":\"area\"}]}"
  throw: true
```
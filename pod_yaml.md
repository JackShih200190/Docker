### yaml 
```
apiVersion
apiVersion 是代表目前 Kubernetes 中該元件的版本號。以上述的例子 Pod 是 v1，而 v1也是目前Kubernetes中核心的版本號。在日後也會陸續看到 betav1, v1alpha1 等版本號，更多 Kubernetes API 的版本號，可至 官網 API versioning查看。

metadata
在 metadata 中，有三個重要的 Key，分別是 name, labels, annotations。

metadata.name
我們可以在 metadata.name 的欄位指定這個 Pod 的名稱，這裡 Pod 的名稱就是 my-pod
metadata.labels
而 metadata.labels 是 Kubernetes 的是核心的元件之一，Kubernetes 會透過 Label Selector 將Pod分群管理。在之後 [Day 10] Kubernetes世界不可缺少的 - Labels 學習筆記中，將會詳細介紹 Labels 的功能。
metadata. annotations
annotations 的功能與 labels 相似。相較於labels，annotations 通常是使用者任意自定義的附加資訊，提供外部進行查詢使用，像是版本號，發布日期等等。
spec
最後 spec 的部分則是定義 container，在這個範例中，一個 Pod 只運行一個 container。

container.name
我們可以在這 container 中設定 container 的名稱
container.image
Image 則是根據 Docker Registry 提供的可下載路徑。
container.ports
最後 ports 的部分則是可以指定，該 container 有哪些 port number 是允許外部資源存取，而在這裡我們只允許container中的port 3000對外開放。
在了解 my-first-pod.yaml 每一行在做什麼事情之後，我們可以使用 kubectl create 指令在 Kubernetes Cluster 中建立 Pod 物件
```

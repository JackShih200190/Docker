### Docker_build
```
OPTIONS說明：
  •	--build-arg=[] :設置鏡像創建時的變數；
  •	--cpu-shares :設置 cpu 使用權重；
  •	--cpu-period :限制 CPU CFS週期；
  •	--cpu-quota :限制 CPU CFS配額；
  •	--cpuset-cpus :指定使用的CPU id；
  •	--cpuset-mems :指定使用的記憶體 id；
  •	--disable-content-trust :忽略校驗，默認開啟；
  •	-f :指定要使用的Dockerfile路徑；
  •	--force-rm :設置鏡像過程中刪除中間容器；
  •	--isolation :使用容器隔離技術；
  •	--label=[] :設置鏡像使用的中繼資料；
  •	-m :設置記憶體最大值；
  •	--memory-swap :設置Swap的最大值為記憶體+swap，"-1"表示不限swap；
  •	--no-cache :創建鏡像的過程不使用緩存；
  •	--pull :嘗試去更新鏡像的新版本；
  •	--quiet, -q :安靜模式，成功後只輸出鏡像 ID；
  •	--rm :設置鏡像成功後刪除中間容器；
  •	--shm-size :設置/dev/shm的大小，預設值是64M；
  •	--ulimit :Ulimit配置。
  •	--squash :將 Dockerfile 中所有的操作壓縮為一層。
  •	--tag, -t: 鏡像的名字及標籤，通常 name:tag 或者 name 格式；可以在一次構建中為一個鏡像設置多個標籤。
  •	--network: 默認 default。在構建期間設置RUN指令的網路模式
```

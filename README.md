


### execution

npm i

npm run dev


### 하셔야 할것

pages/index.js compoentDidMount 참고 하셔서 
line 132 
const position = new naver.maps.LatLng(37.3595704, 127.105399)  
=> const position = new naver.maps.LatLng(this.props.latitude, this.props.longitude) 바꺼주세요

## 문제점

애니메이션: 네이버가 CSS animation을 아예 지원을 안해서 네이버에서 제공하는
Bounce animation을 대신 추가했습니다.

요청하신 info_window/overlay를 네이버에서는 jQuery를 통해서 virtual dom이 아
닌 actual dom에 add를 하게되어 좋은/나쁨 상태 메세지를 더하는 순간 웹사이트가 아예 멈춥니다.

search magnifying glass svg가 잘못된거 같은데 다시 스케치에서 만
드셔서 components/search/search line 207 바꿔주시면 됩니다.
 
### 실행 가능한것

아이피 혹은 로케이션으로 장소 추적 기능,
네이버 줌인/중 아웃/ 센터 기능/
Search는 제가 집접 알고리즘을 짜서 정말 빠르게 잘됩니다.

flow: 유저가 장소를 입력하면 node js에서 보내주신 아마존 백앤드와 네이버 api를 실행 후
가장 가까운 장소를 더해줍니다.





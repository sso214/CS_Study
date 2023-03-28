# 🎯 LinkedList
- - -

LinkedList(링크드리스트)는 자료를 연속된 메모리 공간이 아닌, 각각의 노드가 자신의 다음 노드를 가리키는 방식으로 구현된 자료구조입니다. 각 노드는 데이터와 다음 노드를 가리키는 포인터(주소)로 구성되어 있습니다.

LinkedList는 자료구조의 개념을 이해하기 쉬우며, 추가, 삭제 작업이 빈번한 상황에서는 좋은 성능을 보입니다. 그러나 검색을 빈번하게 수행해야 하는 경우에는 효율성이 떨어지기 때문에, 검색 작업이 더 많은 상황에서는 다른 자료구조를 선택하는 것이 좋습니다.

<br>

### **_LinkedList의 구조_**
- - -

각 노드가 데이터와 포인터를 가지고 한 줄로 연결되어 있는 방식으로 데이터를 저장하는 자료구조이다.

<img width="350" alt="스크린샷 2023-03-26 오후 9 31 46" src="https://user-images.githubusercontent.com/55771326/227775857-40ce018c-dbef-4fd4-8f60-4bd7b80afc2b.png">

<br>

### **_LinkedList 장단점_**
- - -
<span style="font-size: 20px">**⭐️ LinkedList 장점**</span> <br>

1. 삽입과 삭제가 용이합니다
   * 데이터가 포인터로 서로 연결되어 있기 때문에 삽입과 삭제가 매우 빠릅니다. 데이터 요소를 삽입하려면 그 요소를 가리키는 포인터만 수정하면 됩니다. 이는 배열과 달리 해당 인덱스 이후의 모든 데이터를 이동시킬 필요가 없기 때문에 매우 효율적입니다.
2. 유동적인 크기
   * 데이터 요소들이 동적으로 할당되기 때문에 배열과 달리 크기가 제한되지 않습니다. 이는 데이터 요소를 동적으로 추가하거나 삭제하는 애플리케이션에 유용합니다.
3. 메모리 사용이 효율적입니다
   * 포인터로 연결된 노드로 구성되어 있으므로 메모리를 효율적으로 사용할 수 있습니다.

<br>

<span style="font-size: 20px">**💀️ LinkedList 단점**</span> <br>

1. 인덱싱이 어렵습니다
   * 데이터 요소들이 포인터로 연결되어 있기 때문에, 특정 인덱스에 있는 데이터 요소에 직접 액세스하는 것이 불가능합니다. 대신, 데이터 요소들을 하나씩 따라가야만 합니다.
2. 추가적인 메모리 공간 필요
   * 각 노드가 다음 노드를 가리키는 포인터를 가지고 있기 때문에, 배열과 달리 추가적인 메모리 공간이 필요합니다.
3. 순차 액세스가 느립니다
   * 인덱싱이 불가능하기 때문에, 데이터 요소들을 순차적으로 따라가야만 합니다. 이는 배열에 비해 상대적으로 느린 액세스 시간을 유발할 수 있습니다.

<br>


<br>
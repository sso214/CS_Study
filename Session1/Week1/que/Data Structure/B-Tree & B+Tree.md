# 🎯 B-Tree & B+Tree
- - -
B-Tree와 B+Tree는 대용량의 데이터를 관리하기 위한 자료구조로, 데이터베이스나 파일 시스템에서 주로 사용됩니다.

<br>

### **_B-Tree란?_**
- - -
자식 노드의 개수가 일정하게 유지되는 트리입니다. 이진 탐색 트리의 일반화된 형태로, 노드당 키값이 여러개 저장됩니다. B-Tree는 매우 균형잡힌 트리로, 트리의 높이가 작아 검색 시간이 빠릅니다. B-Tree는 블록 단위로 데이터를 저장하는데, 이는 대용량 데이터 처리에 용이합니다.

<br>

### **_B+Tree란?_**
- - -
B-Tree의 변형으로, 내부 노드에는 키값만 저장하고, 리프 노드에만 데이터를 저장합니다. 이로 인해 리프 노드의 개수가 많아지며, 대용량 데이터를 처리하는 데 더욱 효과적입니다. 또한, 범위 검색에 용이하며, 인덱스를 이용한 검색에도 매우 효과적입니다. B+Tree는 대용량 데이터베이스 시스템에서 인덱스로 많이 사용되고 있습니다.

<br>

### **_B-Tree & B+Tree 공통점_**
- - -

1. 모든 리프 노드가 같은 레벨에 위치해 있습니다.
2. 트리의 균형을 유지합니다.
3. 키의 순서에 따라 트리를 구성합니다.
4. 데이터 접근 시간이 상수 시간에 가깝습니다.

<br>

### **_B-Tree & B+Tree 차이점_**
- - -

1. B-Tree는 내부 노드와 리프 노드에 모두 데이터를 저장하지만, B+Tree는 내부 노드에는 키값만을 저장하고 리프 노드에만 데이터를 저장합니다.
2. B-Tree는 키값을 중복해서 저장할 수 있지만, B+Tree는 키값을 중복해서 저장할 수 없습니다.

<br>

### **_B-Tree & B+Tree 장단점_**
- - -

<span style="font-size: 20px">**⭐️ B-Tree 장점**</span> <br>

1. 키값 중복을 허용하기 때문에, 데이터의 추가 및 삭제가 용이합니다.
2. 키값을 정렬한 형태로 트리를 구성하기 때문에, 범위 검색에 유용합니다.
3. 대용량 데이터를 처리하는 데 효과적입니다.

<br>

<span style="font-size: 20px">**💀️ B-Tree 단점**</span> <br>

1. 내부 노드와 리프 노드 모두 데이터를 저장하기 때문에, 저장 공간의 낭비가 발생할 수 있습니다.
2. 키값의 중복을 허용하기 때문에, 검색 시간이 길어질 수 있습니다.

<br>
<br>

<span style="font-size: 20px">**⭐️ B+Tree 장점**</span> <br>

1. 내부 노드에는 키값만을 저장하고, 리프 노드에만 데이터를 저장하기 때문에, 저장 공간의 낭비를 최소화합니다.
2. 리프 노드는 모두 연결 리스트 형태로 구성되어 있기 때문에 범위 검색에 매우 용이합니다.
3. 인덱스를 이용한 검색에 매우 효과적입니다.

<br>

<span style="font-size: 20px">**💀️ B+Tree 단점**</span> <br>

1. 키값 중복을 허용하지 않기 때문에, 데이터의 추가 및 삭제가 어렵습니다.
2. 리프 노드를 제외한 내부 노드는 데이터를 저장하지 않기 때문에, 검색 시간이 B-Tree보다 길어질 수 있습니다.

<br>

따라서, **B-Tree**는 대용량 데이터를 처리하는 데 효과적이며, 범위 검색이 가능하지만 저장 공간의 낭비가 발생할 수 있습니다. **B+Tree**는 저장 공간을 최소화하며, 범위 검색 및 인덱스를 이용한 검색에 효과적이지만, 데이터의 추가 및 삭제가 어려울 수 있습니다. 선택하는 자료구조는 데이터의 특성에 따라 달라지며, 특히 대용량 데이터 처리를 위해서는 자료구조의 장단점을 고려하여 적절한 선택이 필요합니다.
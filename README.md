# CP_for_fun
# Codeforces Round 869 (Div. 1)

A: N/A

B: Graph:

-> # Kỹ thuật kiểm tra có vòng tròn khép kín tại node hay không, 
  - dfs(node, pre_node) 
    + Basic stop: Dừng khi cạnh đi từ 1 điểm khác root tới điểm lân cận của root -> trả về 1;
    + Duyệt dfs_con từ adj:
      Return 1 khi có 1 dfs_con = 1;
      Return 0 khi tất cae dfs_con = 0;
-> # Cách lấy các cạnh của vòng tròn này:
  - Đánh dấu vị trí cuối cùng trong lúc duyệt dfs,
  - Đánh dấu vị trí pre_node trong lúc duyệt dfs,
  - Truy ngược lại từ node cuối cùng về đầu. for(int t=z; t!=root; t=f(t))
  

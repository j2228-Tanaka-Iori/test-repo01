# test-repo01
Web system test repository

# テスト用のファイル
# eDIT tHiS FIlE

```c++
int main(){
  int a;cin>>a;
  dsu uf(a);
  uf.merge(1,5);
  cout<<uf.size(1)<<endl;
  return 0;
}
```


|fff|aaa|
|---|---|
|ringo|onigiri|


$$
\frac{\pi}{e}
$$

# Union find
```c++
struct dsu{
  int n;
  vector<int>par;
  int leader(int u){
    if(par[u]==-1)return u;
    else par[u]=leader(par[u]);
  }
  bool merge(int u,int v){
    u=leader(u), v=leader(v);
    if(u==v)return false;
    par[u]=v;
    return true;
  }
  bool same(int u,int v){
    return leader(u)==leader(v);
  }
}
```

f
# functional graph

```c++
struct Graph{
  int n_;
  vector<vector<int>>G;
  Graph(){}
  Graph(int n):n(n){
    G.resize(n);
  }
};
```
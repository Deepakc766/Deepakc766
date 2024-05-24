#include<iostream>
using namespace std;
#include<vector>
int main(int argc, char const *argv[])
{
    
vector<vector<int> >v={
    {1, 2, 3, 4},
    {5, 6, 7, 8},
    {9, 10, 11, 12},
    {13, 14, 15, 16},
    {17, 18, 19, 20}
};

int row=v.size();
int col=v[0].size();
for(int j=0;j<col;j++){
    for(int i=0;i<row;i++){
        if(j%2==0){
            cout<<v[i][j]<<" ";
        }else{
            cout<<v[row-i-1][j]<<" ";
        }
    }
}

    return 0;
}

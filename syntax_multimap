#include <iostream>
#include <vector>
#include <map>
#include <iterator>
using namespace std;
int main()
{

    vector<int> nums={1,2,1};
    int n=nums.size();
    vector<int> res(n,-1);
    multimap <int, int> gquiz1;
    multimap <int, int> :: iterator itr;
        for(int i=0;i<nums.size(); i++)
        {
            gquiz1.insert(pair <int, int> (nums[i], i));
        }
        for(int i=0; i<nums.size(); i++)
        {
            if(gquiz1.find(nums[i])!= gquiz1.end())
            {
                itr=gquiz1.find(nums[i]);
                while(itr != gquiz1.end())
                {
                    if(nums[i]<itr->first){
                    res[i]=itr->first;
                    break;
                    }
                }
                itr++;
            }
        }
        for (int i = 0; i < res.size(); i++)
        cout << res[i] << " ";
        return 0;
}

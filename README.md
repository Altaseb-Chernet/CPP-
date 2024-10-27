// c++ program using namespace
#include <iostream>

using namespace std;

namespace altaseb{
    
    double oddProduct(int numberLimit){
        
        long double product=1;
        
        for(int i=1;i <= numberLimit; i++){
            if(i%2 == 0){
                product *=i;
            }
        }
        
        cout<<"the product of the number from  1 to "<<numberLimit<<" is = "<<product;
        
        return product;
    }
    
    
    
    
}

int main() {
    int numberLimit;
    cout<<"please enter a number "<<endl;
        cin>>numberLimit;
        
   altaseb::oddProduct(numberLimit);
   
    return 0;
}

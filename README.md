using namespace std;

int main() {
	int n,k;
	cout<<" nhap so lan lap :"; cin>>k;
	cout<<"\n nhap s phan tu :"; cin>>n;
	const int khoi =1000;
	int a[khoi];
	while (k--){
		for (int i=0;i<n;i++){
			cout<<" nhap "<<i<<" :"; cin>>a[i]; cout<<endl;
		}
		int left=0 ;
		int sum=0;
		for (int i=0;i<n;i++){
			sum+=a[i];
		}
		for (int i=0;i<n;i++){
			sum-=a[i];
			if(sum==left){
				cout<<"diem can bang la:"<<i;
				
			}
			left+=a[i];
		}
		

	}
	
return 0; 
}

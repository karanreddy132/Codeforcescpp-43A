# Codeforcescpp-43A
#include <bits/stdc++.h>
using namespace std;

int main() {
	int n, first(1), second(0);
	cin >> n;
	string s[101], tmp;
	cin >> s[0];
	for (int i = 1; i < n; i++) {
		cin >> s[i];
		if (s[i].compare(s[0]) == 0)
			first++;
		else {
			tmp = s[i];
			second++;
		}
	}
	cout << ((first > second) ? (s[0]) : (tmp));
	return 0;
}

#include <cmath>
#include <cstdio>
#include <vector>
#include <iostream>
#include <algorithm>
using namespace std;


struct User {
    int userID;
    int balance;
};

bool compareUsers(const User &a, const User &b) {
    return a.balance < b.balance || (a.balance == b.balance && a.userID < b.userID);
}

int main() {
    int N;
    cin >> N;

    vector<User> users(N);
    for (int i = 0; i < N; i++) {
        cin >> users[i].userID >> users[i].balance;
    }

    int T;
    cin >> T;

    for (int i = 0; i < T; i++) {
        int from_userID, to_userID, amount;
        cin >> from_userID >> to_userID >> amount;

        int fromIndex = -1, toIndex = -1;
        for (int j = 0; j < N; j++) {
            if (users[j].userID == from_userID) fromIndex = j;
            if (users[j].userID == to_userID) toIndex = j;
        }

        if (fromIndex != -1 && toIndex != -1 && users[fromIndex].balance >= amount) {
            users[fromIndex].balance -= amount;
            users[toIndex].balance += amount;
            cout << "Success" << endl;
        } else {
            cout << "Failure" << endl;
        }
    }

    sort(users.begin(), users.end(), compareUsers);
    cout<<endl;
    for (const auto &user : users) {
        
        cout <<user.userID << " " << user.balance << endl;
    }

    return 0;
}

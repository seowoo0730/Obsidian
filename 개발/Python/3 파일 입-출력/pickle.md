```Python
import pickle
profile_file = open('profile.pickle', 'wb')
profile = {'name': '이서우', 'age': '14'}
pickle.dump(profile, profile_file)  # profile을 profile_file에 저장
profile_file.close()
```

```Python
import pickle
profile_file = open('profile.pickle', 'rb')  # profile_file 열기
profile = pickle.load(profile_file)  # profile을 profile_file에서 불러온 값으로
print(profile)
#{'name': '이서우', 'age': '14'}
```

### `with`

```Python
import pickle

with open('profile.pickle', 'rb') as profile_file:  # profile.pickle을 profile_file에 할당
    print(pickle.load(profile_file))
# {'name': '이서우', 'age': '14'}
```
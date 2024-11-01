
# Git ბრძანებების სია

ეს ფაილი შეიცავს Git-ის ძირითადი ბრძანებების აღწერას და განმარტებებს.

## 1. გიტის კონფიგურაცია
- `git config --global user.name "თქვენი სახელი"` – ქმნის მომხმარებლის სახელს ყველა პროექტისთვის. (კონფიგს ქმნის გლობალურს)
- `git config --global user.email "თქვენი ელ.ფოსტა"` – ქმნის მომხმარებლის ელ.ფოსტას ყველა პროექტისთვის. (კონფიგს ქმნის გლობალურს) 

## 2. ახალი რეპოზიტორიის შექმნა
- `git init` – ქმნის ახალ Git რეპოზიტორიას მოცემულ დირექტორიაში.

## 3. GitHub რეპოზიტორიასთან დაკავშირება
- `git remote add origin [url]` – აკავშირებს ლოკალურ რეპოზიტორიას დისტანციურ (GitHub) რეპოზიტორიასთან.

## 4. ცვლილებების დათვალიერება
- `git status` – აჩვენებს მიმდინარე ცვლილებების სტატუსს.
- `git diff` – აჩვენებს განსხვავებებს (ცვლილებებს), რომლებიც ჯერ არ არის „staged“.
- `git diff --staged` – აჩვენებს „staged“ მდგომარეობაში მყოფი ფაილების ცვლილებებს.

## 5. ფაილების მომზადება (Staging)
- `git add [file]` – გადაყავს კონკრეტულ ფაილს „staged“ მდგომარეობაში commit-ისთვის.
- `git add .` – გადაყავს ყველა შეცვლილ ფაილს „staged“ მდგომარეობაში.

## 6. Commit-ის შექმნა
- `git commit -m "Commit-ის შეტყობინება"` – ქმნის commit-ს „staged“ ფაილებისგან.
- `git commit -a -m "Commit-ის შეტყობინება"` – აერთიანებს ყველა ცვლილებას „staged“-ის გარეშე და ქმნის commit-ს.

## 7. ლოგის დათვალიერება
- `git log` – აჩვენებს commit-ების ისტორიას.
- `git log --oneline` – აჩვენებს commit-ების მოკლე ისტორიას.
- `git log --stat` – აჩვენებს commit-ების ისტორიას და თითო commit-ისთვის ცვლილებების რაოდენობას.

## 8. განსხვავებების დათვალიერება
- `git show [commit-id]` – აჩვენებს კონკრეტული commit-ის დეტალებს.
- `git diff [commit-id1] [commit-id2]` – აჩვენებს განსხვავებებს ორ commit-ს შორის.

## 9. ფაილების აღდგენა
- `git checkout -- [file]` – აბრუნებს კონკრეტულ ფაილს ბოლო commit-ის ვერსიაზე.
- `git checkout [commit-id] -- [file]` – აბრუნებს ფაილს კონკრეტული commit-ის ვერსიაზე.
- `git reset HEAD [file]` – „unstage“-ში აბრუნებს ფაილს.

## 10. ფაილების წაშლა
- `git rm [file]` – შლის ფაილს Git-დან და სამუშაო დირექტორიიდან.
- `git rm --cached [file]` – შლის ფაილს მხოლოდ Git-დან.

## 11. ფილიალების მართვა
- `git branch` – აჩვენებს ყველა ფილიალს.
- `git branch [branch-name]` – ქმნის ახალ ფილიალს.
- `git checkout [branch-name]` – გადადის კონკრეტულ ფილიალზე.
- `git checkout -b [branch-name]` – ქმნის ახალ ფილიალს და გადადის მასზე.

## 12. ფილიალების შერწყმა (Merge)
- `git merge [branch-name]` – აერთიანებს მითითებულ ფილიალს მიმდინარე ფილიალში.

## 13. რეპოზიტორიის განახლება და ატვირთვა
- `git push` – ატვირთავს ცვლილებებს დისტანციურ რეპოზიტორიაში.
- `git pull` – ჩამოტვირთავს და აერთიანებს დისტანციურ ცვლილებებს.

## 14. Reset და Revert
- `git reset --hard [commit-id]` – აბრუნებს რეპოზიტორიას კონკრეტულ commit-ის მდგომარეობაზე.
- `git revert [commit-id]` – ქმნის ახალ commit-ს, რომელიც აუქმებს კონკრეტული commit-ის ცვლილებებს.



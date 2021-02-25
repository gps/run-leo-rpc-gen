# Leo-RPC-Gen

A Github Action that uses Leo RPC Gen to generate RPC artifacts & publish them.

Note that if you plan to generate Kotlin code, it is assumed that you have already installed an appropriate JDK.

For example, before running this action you should have included:

```yml
- name: Set up JDK 1.8
  uses: actions/setup-java@v1
  with:
    java-version: 1.8
```

It is also recommended that you warm up gradle caches with:

```yml
- name: Warm Up Gradle Caches
  uses: actions/cache@v1
  with:
    path: ~/.gradle/caches
    key: ${{ runner.os }}-gradle-${{ hashFiles('**/*.gradle*') }}
    restore-keys: |
      ${{ runner.os }}-gradle-
```

TODO: Write Documentation on how to use this action.

### Hi there 👋
https://www.google.com/amp/s/www.geeksforgeeks.org/and
<!--
**sahilkhan3122/sahilkhan3122** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.
https://www.google.com/amp/s/www.geeksforgeeks.org/android-session-management-with-kotlin/amp/
Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->




<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent">

    <androidx.constraintlayout.widget.Guideline
        android:id="@+id/guideline_start"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:orientation="vertical"
        app:layout_constraintGuide_begin="@dimen/dimen_20dp" />

    <androidx.constraintlayout.widget.Guideline
        android:id="@+id/guideline_end"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:orientation="vertical"
        app:layout_constraintGuide_end="@dimen/dimen_20dp" />

    <androidx.constraintlayout.widget.Guideline
        android:id="@+id/guideline_bottom"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:orientation="horizontal"
        app:layout_constraintGuide_end="@dimen/dimen_30dp" />

    <androidx.constraintlayout.widget.Guideline
        android:id="@+id/guideline_top"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:orientation="horizontal"
        app:layout_constraintGuide_begin="@dimen/dimen_10dp" />

    <androidx.constraintlayout.widget.Guideline
        android:id="@+id/guideline_divider"
        android:layout_width="0dp"
        android:layout_height="0dp"
        android:orientation="horizontal"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintGuide_begin="366dp"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <androidx.appcompat.widget.AppCompatButton
        android:id="@+id/btn_1"
        android:layout_width="0dp"
     android:text="test"
        style="@style/button_style"
        android:layout_height="wrap_content"
        app:layout_constraintEnd_toStartOf="@+id/guideline_end"
        app:layout_constraintStart_toEndOf="@id/guideline_start"
        app:layout_constraintTop_toBottomOf="@+id/guideline_top" />

    <androidx.appcompat.widget.AppCompatButton
        android:id="@+id/btn_2"
        android:layout_width="0dp"
        style="@style/button_style"
        android:layout_height="wrap_content"
        android:layout_marginTop="@dimen/dimen_20dp"
        app:layout_constraintEnd_toStartOf="@+id/guideline_end"
        app:layout_constraintStart_toEndOf="@id/guideline_start"
        app:layout_constraintTop_toBottomOf="@+id/btn_1" />

    <androidx.appcompat.widget.AppCompatButton
        android:id="@+id/btn_3"
        android:layout_width="0dp"
        style="@style/button_style"
        android:layout_height="wrap_content"
        android:layout_marginTop="@dimen/dimen_20dp"
        app:layout_constraintEnd_toStartOf="@+id/guideline_end"
        app:layout_constraintStart_toEndOf="@id/guideline_start"
        app:layout_constraintTop_toBottomOf="@+id/btn_2" />

    <androidx.appcompat.widget.AppCompatButton
        android:id="@+id/btn_4"
        android:layout_width="0dp"
        style="@style/button_style"
        android:layout_height="wrap_content"
        android:layout_marginTop="@dimen/dimen_20dp"
        app:layout_constraintEnd_toStartOf="@+id/guideline_end"
        app:layout_constraintStart_toEndOf="@id/guideline_start"
        app:layout_constraintTop_toBottomOf="@+id/btn_3" />

    <androidx.appcompat.widget.AppCompatButton
        android:id="@+id/btn_test"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:textAllCaps="true"
        style="@style/button_style"
        android:layout_margin="@dimen/dimen_10dp"
        app:layout_constraintBottom_toBottomOf="@+id/guideline_divider"
        app:layout_constraintEnd_toStartOf="@+id/guideline_end"
        app:layout_constraintStart_toEndOf="@+id/guideline_start"
        app:layout_constraintTop_toTopOf="@+id/guideline_divider"
        tools:text="test" />

    <androidx.appcompat.widget.AppCompatImageView
        android:id="@+id/imageView"
        android:layout_width="wrap_content"
        android:layout_height="@dimen/dimen_30dp"
        android:layout_marginTop="@dimen/dimen_40dp"
        android:background="@drawable/ic_launcher_foreground"
        app:circularflow_angles="180"
        app:layout_constraintBottom_toBottomOf="@+id/btn_test"
        app:layout_constraintCircle="@+id/btn_test"
        app:layout_constraintCircleRadius="10dp"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="@+id/btn_test" />

    <androidx.constraintlayout.widget.Group
        android:id="@+id/myGroup"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:visibility="visible"
        app:constraint_referenced_ids="btn_1,btn_2,btn_3,btn_4" />


</androidx.constraintlayout.widget.ConstraintLayout>

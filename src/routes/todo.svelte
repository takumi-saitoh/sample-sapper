<script>
    import TaskForm from '../components/TaskForm'
</script>

<style>
.header-title {
    font-weight: lighter;
    font-size: 3.5rem;
}
.main-container{
    padding-bottom: 50px;
}
@media (max-width: 991px) {
    .task-container {
        margin-bottom: 2rem;
    }
}
.task-form-container {
    border-radius: 0.25rem;
}
</style>

<svelte:head>
	<title>TODO APP</title>
</svelte:head>
<div class="container">
    <header>
        <h1 class="header-title">TO DO APP</h1>
    </header>
    <div class="row main-container">
        <div class="col-md-8 col-xl-9 task-container">
            <div class="task-form-container bg-dark">
            <TaskForm />
            </div>
        </div>
        <div class="col-md-4 col-xl-3">
        bbb
        </div>
    </div>
</div>

<template>
  <form class="w-full max-h-lg m-8">
    <fieldset>
      <legend class="sr-only">Countries</legend>

      <h2 class="text-3xl text-left font-bold">Search Invoice</h2><br>

      <div class="flex items-center mb-4">
        <input id="default-radio-1" type="radio" value="" name="default-radio"
          class="w-4 h-4 text-blue-600 bg-gray-100 border-gray-300 focus:ring-blue-500 dark:focus:ring-blue-600 dark:ring-offset-gray-800 focus:ring-2 dark:bg-gray-700 dark:border-gray-600">
        <label for="default-radio-1" class="ml-2 text-sm font-bold text-gray-900 dark:text-gray-300">General
          Enquiry</label>
      </div>
      <div class="flex items-center">
        <input checked id="default-radio-2" type="radio" value="" name="default-radio"
          class="w-4 h-4 text-blue-600 bg-gray-100 border-gray-300 focus:ring-blue-500 dark:focus:ring-blue-600 dark:ring-offset-gray-800 focus:ring-2 dark:bg-gray-700 dark:border-gray-600">
        <label for="default-radio-2" class="ml-2 text-sm font-bold text-gray-900 dark:text-gray-300">Exact
          Match</label>
      </div><br>

      <div class="flex flex-wrap -mx-3 mb-6">
        <div class="w-full md:w-1/3 px-3 mb-6 md:mb-0">
          <label class="block text-left tracking-wide text-gray-700 text-xs font-bold mb-2" for="grid-first-name">
            Invoice Number
          </label>
          <input
            class="appearance-none block w-full h-15 bg-white text-gray-700 border border-gray-500 rounded py-3 px-4 leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
            id="grid-last-name" type="text">
        </div>
        <div class="w-full md:w-2/12 px-3">
          <label class="block tracking-wide text-left  text-gray-700 text-xs font-bold mb-2" for="grid-last-name">
            Invoice Date
          </label>
          <input
            class="appearance-none block w-full h-15 bg-white text-gray-700 border border-gray-500 rounded py-3 px-4 leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
            id="grid-last-name" type="date">
        </div>
        <div class="w-full px-3 md:w-2/12 mb-6 md:mb-0">
          <label class="block tracking-wide text-left text-gray-700 text-xs font-bold mb-2" for="grid-password">
            Invoice Type
          </label>
          <select
            class="block appearance-none w-full h-15 bg-white text-gray-700 border border-gray-500 py-3 px-4 pr-8 rounded leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
            id="grid-state">
            <option></option>
            <option>New Mexico</option>
            <option>Missouri</option>
            <option>Texas</option>
          </select>
        </div>
        <div class="w-full md:w-2/12 px-3 mb-6 md:mb-0">
          <label class="block tracking-wide text-left text-gray-700 text-xs font-bold mb-2" for="grid-city">
            Bank Reference Number
          </label>
          <input
            class="appearance-none block w-full h-15 bg-white text-gray-700 border border-gray-500 rounded py-3 px-4 leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
            id="grid-city" type="text">
        </div>
      </div>

      <div class="flex flex-wrap -mx-3 mb-2">
        <div class="w-full md:w-2/12 px-3 mb-6 md:mb-0">
          <label class="block tracking-wide text-left text-gray-700 text-xs font-bold mb-2" for="grid-state">
            Invoice Amount
          </label>
          <input
            class="appearance-none block w-full h-15 bg-white text-gray-700 border border-gray-500 rounded py-3 px-4 leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
            id="grid-city" type="text">
        </div>
        <div class="w-full md:w-2/12 px-3 mb-6 md:mb-0">
          <label class="block tracking-wide text-left text-gray-700 text-xs font-bold mb-2" for="grid-last-name">
            Invoice Recorded Date
          </label>
          <input
            class="appearance-none block w-full h-15 bg-white text-gray-700 border border-gray-500 rounded py-3 px-4 leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
            id="grid-last-name" type="date">
        </div>
        <div class="w-full md:w-1/3 px-3 mb-6 md:mb-0">
          <label class="block uppercase tracking-wide text-left text-gray-700 text-xs font-bold mb-2" for="grid-zip">
            BRN
          </label>
          <input
            class="appearance-none block w-full h-15 bg-white text-gray-700 border border-gray-500 rounded py-3 px-4 leading-tight focus:outline-none focus:bg-white focus:border-gray-500"
            id="grid-zip" type="text">
        </div>

        <button class="bg-blue-700 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded-lg m-4 w-44 h-12">
          Reset
        </button>
        <button class="bg-blue-700 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded-lg m-4 w-44 h-12">
          Search
        </button>
      </div><br><br>

      <div class="overflow-x-auto relative shadow-md sm:rounded-lg">
        <table class="w-full text-sm text-left text-gray-500 dark:text-gray-400">
          <thead class="text-xs text-gray-700 uppercase bg-gray-200 dark:bg-gray-700 dark:text-gray-400">
            <tr>
              <th scope="col" class="py-3 px-6">
                status
              </th>
              <th scope="col" class="py-3 px-6">
                invoice id
              </th>
              <th scope="col" class="py-3 px-6">
                invoice number
              </th>
              <th scope="col" class="py-3 px-6">
                invoice date
              </th>
              <th scope="col" class="py-3 px-6">
                invoice type
              </th>
              <th scope="col" class="py-3 px-6">
                invoice amount
              </th>
              <th scope="col" class="py-3 px-6">
                Action
              </th>
            </tr>
          </thead>
          <tbody>
            <tr class="bg-white border-b dark:bg-gray-900 dark:border-gray-700">
              <th>

              </th>
              <td class="py-4 px-6">
                Apple MacBook Pro 17"
              </td>
              <td class="py-4 px-6">
                Sliver
              </td>
              <td class="py-4 px-6">
                Laptop
              </td>
              <td class="py-4 px-6">
                $2999
              </td>
              <td class="py-4 px-6">
                $2999
              </td>
              <td class="py-4 px-6">
                <a href="#" class="font-medium text-blue-600 dark:text-blue-500 hover:underline">View</a><br>
                <a href="#" class="font-medium text-blue-600 dark:text-blue-500 hover:underline">Edit</a><br>
                <a href="#" class="font-medium text-blue-600 dark:text-blue-500 hover:underline">Delete</a>
              </td>
            </tr>
            <tr class="bg-white border-b dark:bg-gray-900 dark:border-gray-700">
              <th>

              </th>
              <td class="py-4 px-6">
                Apple MacBook Pro 17"
              </td>
              <td class="py-4 px-6">
                Sliver
              </td>
              <td class="py-4 px-6">
                Laptop
              </td>
              <td class="py-4 px-6">
                $2999
              </td>
              <td class="py-4 px-6">
                $2999
              </td>
              <td class="py-4 px-6">
                <a href="#" class="font-medium text-blue-600 dark:text-blue-500 hover:underline">View</a><br>
                <a href="#" class="font-medium text-blue-600 dark:text-blue-500 hover:underline">Edit</a><br>
                <a href="#" class="font-medium text-blue-600 dark:text-blue-500 hover:underline">Delete</a>
              </td>
            </tr>
            <tr class="bg-white border-b dark:bg-gray-900 dark:border-gray-700">
              <th>

              </th>
              <td class="py-4 px-6">
                Apple MacBook Pro 17"
              </td>
              <td class="py-4 px-6">
                Sliver
              </td>
              <td class="py-4 px-6">
                Laptop
              </td>
              <td class="py-4 px-6">
                $2999
              </td>
              <td class="py-4 px-6">
                $2999
              </td>
              <td class="py-4 px-6">
                <a href="#" class="font-medium text-blue-600 dark:text-blue-500 hover:underline">View</a><br>
                <a href="#" class="font-medium text-blue-600 dark:text-blue-500 hover:underline">Edit</a><br>
                <a href="#" class="font-medium text-blue-600 dark:text-blue-500 hover:underline">Delete</a>
              </td>
            </tr>
            <tr class="bg-white border-b dark:bg-gray-900 dark:border-gray-700">
              <th>

              </th>
              <td class="py-4 px-6">
                Apple MacBook Pro 17"
              </td>
              <td class="py-4 px-6">
                Sliver
              </td>
              <td class="py-4 px-6">
                Laptop
              </td>
              <td class="py-4 px-6">
                $2999
              </td>
              <td class="py-4 px-6">
                $2999
              </td>
              <td class="py-4 px-6">
                <a href="#" class="font-medium text-blue-600 dark:text-blue-500 hover:underline">View</a><br>
                <a href="#" class="font-medium text-blue-600 dark:text-blue-500 hover:underline">Edit</a><br>
                <a href="#" class="font-medium text-blue-600 dark:text-blue-500 hover:underline">Delete</a>
              </td>
            </tr>
          </tbody>
        </table>
      </div>

    </fieldset>
  </form>
</template>

<script>
export default {

}
</script>
